# Secure Image Steganography 

The idea:
- hide secret messages inside images
- encrypt the message before hiding it
- recover it later using a decryption key

Still improving it gradually. Current build is around the “March → April update” phase.

---

## Current Features

- AES-based encryption using Fernet
- Message embedding inside images
- GUI application using Tkinter
- Native file picker support
- Encode / Decode workflow
- Secret key generation
- Save encrypted image anywhere locally
- Cross-platform file dialog support (Linux/Windows/macOS)

---

## Tech Stack

- Python
- OpenCV (`cv2`)
- Tkinter
- Cryptography (Fernet)
- NumPy
- Pillow

---

## Project Status

Working prototype.

Main functionality works properly:
- encryption
- embedding
- extraction
- decryption

Still refining:
- embedding algorithm
- UI cleanup
- error handling
- optimization
- better steganography techniques

---

## Important Note

Current implementation is more focused on:
- learning
- functionality
- workflow

than perfect steganographic stealth.

Right now the project uses direct pixel value embedding, not advanced LSB randomization yet. Planning to improve this in future updates.

---

## Installation

Clone the repo:

```bash
git clone https://github.com/anisa-droid/Secure-Image-Steganography-Project.git
```

Install dependencies:

```bash
pip install opencv-python cryptography numpy pillow
```

Run:

```bash
python stego_gui_april_update_1.01.py
```

---

## How it Works

### Encryption Flow

```text
Message
   ↓
Fernet Encryption
   ↓
Base64 Encoding
   ↓
Embedded into Image Pixels
   ↓
Encrypted Image Output
```

### Decryption Flow

```text
Encrypted Image
   ↓
Extract Embedded Data
   ↓
Base64 Decode
   ↓
Fernet Decryption
   ↓
Original Message
```

---

## Screenshots

(Will be adding real soon)

---

## Future Plans

- Better image capacity handling
- Executable build
- Drag & drop support
- More secure key management

---
