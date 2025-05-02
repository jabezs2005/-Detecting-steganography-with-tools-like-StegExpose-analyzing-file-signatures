# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands
# Step 1: Download Image and Create Secret Message File
• Download a .jpeg image  from a trusted website or use own image.
![Screenshot 2025-05-02 212523](https://github.com/user-attachments/assets/f4c37e4a-a63c-4a75-849c-7e7a3d2543cf)
• Create a text file named secret with a confidential message:
![Screenshot 2025-05-02 212537](https://github.com/user-attachments/assets/de6dc9e6-886c-4052-b641-d893cf0c6e5a)
# Step 2: Install and Verify Steghide Tool
• To install Steghide on Kali linux,run:

• Confirm the installation by checking its version:
![Screenshot 2025-05-02 212551](https://github.com/user-attachments/assets/04fbbbc3-1620-40de-8931-9b02477b464c)

# Step 3: Embed the Secret Message into the Image
• Use the following command to embed secret into praveen.jpeg:
![Screenshot 2025-05-02 212612](https://github.com/user-attachments/assets/1a5edff3-3681-42e4-9272-e6d19c712ab1)
# Step 4: Delete the Original Secret File
• After embedding, delete the plaintext file:
## OUTPUT:
List of Images with Steganography Detection Scores and File Signature Details
![Screenshot 2025-05-02 212624](https://github.com/user-attachments/assets/ce6309b0-45a5-4145-8c3c-ec20aea91cf2)
## OUTPUT:
List of Images with Steganography Detection Scores and File Signature Details

# Step 1: Extract the Embedded Secret from the Image
![Screenshot 2025-05-02 212642](https://github.com/user-attachments/assets/34f788d4-1bb1-46e3-8087-521939e6ea5a)
• To retrieve the hidden file:
• Enter the same passphrase used during embedding.
![Screenshot 2025-05-02 212657](https://github.com/user-attachments/assets/d2bf5113-372e-47a3-b47b-ab40c8fb2ba8)
# Step 2: Verify the Extracted Message
• Display the extracted file content to verify:

• Ensure the message matches the original secret content.

• Another command to see the same secret message is

# Step 3: Retrieve Information About the Embedded Data
• To gather details about embedded content in the image:
![Screenshot 2025-05-02 212713](https://github.com/user-attachments/assets/665b6483-3ad5-4c51-a1ef-9e7a6aa0cbd4)
• This will display file type, size, and whether data is embedded.
## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
