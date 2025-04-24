# EXP8:DETECTING STEGANOGRAPHY WITH TOOLS  LIKE STEGEXPOSE,ANALYSING FILE SIGNATURES

## AIM:
To hide and extract secret information (e.g., text files) inside a cover file (e.g., JPEG image) using the steganography tool `steghide` in Kali Linux.

EQUIPMENTS REQUIRED:
●	Hardware: PCs

```
Register Number: 212222040128
Name: RAGHUL S

```

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., praveen.jpeg) from a trusted website or use own image.
  
  ![8 1](https://github.com/user-attachments/assets/6beb4fc2-1dba-439f-af93-4e834fd1bf05)

  
  •	Create a text file named secret with a confidential message:
  
![8 2](https://github.com/user-attachments/assets/09f7d239-fb87-4e80-8055-af5f29990f22)
![8 3](https://github.com/user-attachments/assets/71386a9b-62da-4e10-95ff-96a26a21909f)




### Step 2: Install and Verify Steghide Tool
  •	To install Steghide on Kali linux,run:
  
  
  •	Confirm the installation by checking its version:
  
  ![8 5](https://github.com/user-attachments/assets/a8d3e25d-3796-4c85-8246-138051919aa6)


 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:
  
![8 6](https://github.com/user-attachments/assets/2c8da8e1-ead9-4e5a-a0ac-2262ba397f0c)



### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
![8 7](https://github.com/user-attachments/assets/382798e2-c4cf-46aa-be39-dd0bb3959f1b)


## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
![8 8](https://github.com/user-attachments/assets/0023dd6b-36a3-409b-ae7d-5bd4c32e1b40)


  •	Enter the same passphrase used during embedding.
  
![8 9](https://github.com/user-attachments/assets/fe643a9f-415d-457f-b956-d27a028e1af9)



### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
![8 10](https://github.com/user-attachments/assets/841219ed-a642-49f1-a41d-e7187c786e90)

  
  •	Ensure the message matches the original secret content.
  
  •	Another command to see the same secret message is
  
![8 11](https://github.com/user-attachments/assets/09436520-aea1-459a-a06c-5d26b4ddc597)


 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
![8 12](https://github.com/user-attachments/assets/7b62cd63-0e42-499a-ba61-a99fb51e2a1a)

  
   
  •	This will display file type, size, and whether data is embedded.

 
## RESULT:
Embedded "secret" into praveen.jpeg successfully using Steghide with passphrase 12345.Extracted and verified hidden message
