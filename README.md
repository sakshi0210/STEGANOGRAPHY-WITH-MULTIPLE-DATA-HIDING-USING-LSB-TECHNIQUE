# Steganography With Multiple Data Hiding Using LSB Techniques

##  Project Overview
This project implements **steganography techniques** to securely hide confidential information inside **images and videos** using the **Least Significant Bit (LSB)** method.  
The system supports **multiple data hiding**, including:
- Text in Image
- Image in Image
- Text/Image in Video  

A **Python-based GUI** is developed to make the system user-friendly and easy to operate.

---

##  Problem Statement
In many domains such as **military, government, and research**, secure communication of confidential data is crucial.  
Traditional encryption reveals the existence of hidden communication, whereas **steganography conceals the very presence of the message**.

This project aims to build a system that hides data inside multimedia files without attracting suspicion.

---

##  Technologies Used
- **Programming Language:** Python  
- **Tools:** Jupyter Notebook  
- **Concepts:**  
  - Digital Image Processing (DIP)  
  - Digital Signal Processing (DSP)  
  - Least Significant Bit (LSB) Technique  
- **Interface:** Graphical User Interface (GUI)

---

## 🔍 Methodology

### 1️⃣ Text Steganography
- Converts text into ASCII values
- Embeds binary data into the **LSB of RGB pixel values**
- Extracts text by reading LSBs during decoding
  <img width="658" height="314" alt="Image" src="https://github.com/user-attachments/assets/565c4c62-40ca-47e3-a4ec-cc1d2ca128f3" />

### 2️⃣ Image Steganography
- Takes **2 MSB bits** of the secret image
- Embeds them into **2 LSB bits** of the cover image
- Reconstructs the secret image during decoding
<img width="608" height="364" alt="Image" src="https://github.com/user-attachments/assets/a5420e55-bf03-4eb6-8353-8fc5effb6a2d" />

### 3️⃣ Video Steganography
- Breaks video into frames
- Embeds text/image data into individual frames using LSB
- Regenerates the video after embedding
<img width="632" height="320" alt="Image" src="https://github.com/user-attachments/assets/b183c001-9147-4e14-b40d-5b5a5dd09b71" />
---

##  Algorithms Used

### Encoding
1. Input cover image/video
2. Convert secret data to binary
3. Embed data into LSB of pixels
4. Regenerate stego image/video
   
Encoding flow:
Input Text
   ↓
Split text into chunks
   ↓
Video → Frames
   ↓
Hide text chunks into frames (LSB)
   ↓
Frames → Video
   ↓
Audio merged back
### Decoding
1. Input stego image/video
2. Extract LSB values
3. Reconstruct original hidden data

Decoding flow:
Video
   ↓
Extract frames
   ↓
Read hidden text from frames
   ↓
Original message recovered

##  Results & Analysis
- Successfully hides **text, image, and video data**
- No noticeable distortion in cover media
- GUI allows easy selection of steganography type
- Maintains data integrity and confidentiality

---

##  Real-World Applications
- Military communication
- Government data transfer
- Research data protection
- Digital watermarking
- Copyright protection

---

##  Future Scope
- Implement advanced techniques such as:
  - DWT (Discrete Wavelet Transform)
  - DCT (Discrete Cosine Transform)
  - DFT (Discrete Fourier Transform)
  - Pixel Value Differencing (PVD)
- Improve accuracy and robustness
- Enhance resistance to steganalysis

---

##  Conclusion
The proposed system successfully demonstrates **secure and efficient data hiding** using LSB-based steganography.  
Compared to image steganography, **video steganography allows higher data capacity and better security**.  
The Python GUI makes the system intuitive and practical for real-world use.

---

##  Author
**Sakshi Vispute**  
Bachelor of Engineering – Electronics & Telecommunication  
Internship at **Indian Institute of Technology Bombay (IITB)**  
Academic Year: 2021–22

---

##  References
1. Mritha Ramalingam, *Video Steganography using Modified LSB Algorithm*, 2011  
2. Amit Singh et al., *Digital Watermarking using LSB*, 2013  
3. Kousik Dasgupta et al., *Hash-based LSB Video Steganography*, 2012  
4. Mehdi Hussain, *Survey of Image Steganography Techniques*, 2013  

---

