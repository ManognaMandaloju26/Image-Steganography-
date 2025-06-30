
# 🖼️ Image Steganography - Hide Text in Image

This project implements **image steganography** using the **Least Significant Bit (LSB)** technique to hide text messages inside PNG images. It provides a simple GUI-based tool to securely **embed** and **extract** secret messages from images without any noticeable change in appearance.

## 📌 Problem Statement

With growing concerns over data privacy, this project offers a solution for discreet communication. By embedding textual data at the binary level within image pixels using the LSB method, it ensures confidential message transmission without relying on traditional encryption methods.

## 💻 System Requirements

* **Python**: 3.10+
* **Libraries**:

  * `tkinter` – GUI development
  * `Pillow` – Image processing

## 🧰 Tools & Technologies

* **Language**: Python
* **Image Format**: PNG
* **Steganography Method**: Least Significant Bit (LSB)
* **GUI**: Tkinter

## ⚙️ Features

* Embed a secret message into a PNG image
* Extract hidden messages from stego-images
* Intuitive and beginner-friendly GUI
* Binary-level data hiding for improved stealth

## 🧠 Algorithm Overview

### 🔐 Hiding Text (`hide_text.py`)

1. User selects a PNG image through the GUI.
2. Text is converted to binary using `text_to_bin()`.
3. Binary is embedded in image pixels' LSBs.
4. An EOF marker (`1111111111111110`) is added.
5. A new image is saved with the hidden message.

### 🔓 Extracting Text (`extract_text.py`)

1. User selects the stego-image using the GUI.
2. LSBs are extracted from image pixels.
3. Binary data is collected until EOF marker is found.
4. Message is reconstructed using `bin_to_text()`.

## 🚀 Deployment

```bash
# To embed text into image
python hide_text.py

# To extract hidden text
python extract_text.py
```

## 📸 Demo & Repository

Check out the project here:
👉 [GitHub Repository](https://github.com/ManognaMandaloju26/Image-Steganography-.git)

## ✅ Results

The project successfully embeds and retrieves hidden messages without visibly altering the image, proving the effectiveness of LSB steganography in real-world applications.

## 🏁 Conclusion

This tool shows how steganography can serve as a lightweight, secure method of secret communication. Its GUI makes it accessible even to non-technical users.

## 🌱 Future Scope

* Support additional image formats (JPG, BMP)
* Password-protected message embedding
* Allow hiding of entire files (not just text)

## 📚 References

* Python Official Documentation
* Pillow Library Docs
* Research articles on Steganography
* GitHub repositories
* Stack Overflow (debugging)

