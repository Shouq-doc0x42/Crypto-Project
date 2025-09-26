# MITM Attack on Diffie–Hellman (FC421 Applied Cryptography – Fall 2025)

<div align="center">
  
[![License: MIT](https://img.shields.io/badge/License-MIT-8e44ad?style=for-the-badge&logo=ghost)](https://opensource.org/licenses/MIT)
![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=yellow)
![Repo Size](https://img.shields.io/github/repo-size/Shouq-doc0x42/Crypto-Project?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-linux%20%7C%20windows-lightgrey?style=for-the-badge&logo=linux)

</div>

## 📌 Project Overview
This project Illustrate the vulnerability of the **Diffie–Hellman (DH) key exchange** to a **Man-in-the-Middle (MITM) attack** when authentication element is missing.
It covers the following components:

- A simple client–server chat system (Eddie ↔ Venom) establishing a symmetric key using DH and encrypt messages with AES.
- An attacker (Mallory) positions himself as a proxy, intercepting both of exchange and creating separate keys with each party. This able him to read or modify messages.
- A defense mechanism can be implemented by adding **RSA digital signatures** to authenticate the DH values, avoiding Mallory from performing a successful attack.

This project is developed as part of **FC421 Applied Cryptography – Fall 2025** at the UPM AKA University of Prince Mugrin.

---
## 📝 MITM Flow Diagram
A simple diagram that has been used in the project:

<div align="center">
  
![Alt text](https://github.com/Shouq-doc0x42/Crypto-Project/blob/main/docs/MITM%20Diagram.png/?raw=true)

</div>



---

## ⚠ Disclaimer
- This project is for **educational purposes only** under the FC421 Applied Cryptography course.
- The character names *Eddie, Venom, Knull (image)* are used as **fictional placeholders** to represent the following client and server roles.
- They're inspired by standard cryptography teaching conventions and popular culture references.
- The use of these names is strictly for **academic demonstration only** and for **non-commercial** purposes.
- I do not own or claim any rights to Marvel characters or other fictional elements.

---

## 👥 Team Members
The people who contributed in the project:
- **Shouq** – Project Manager  
- **Lama** – TBA
- **Omnia** – TBA  

---

## 🛠 Tools & Requirements

## Hardware Requirements

<div align="center">
  
| Components      | Minimum     | Recommended
|-------:|:-----------------------:|:------------
| Processor       | Intel Core i3 or equivilent | Intel Core i5/i7 or equivalent |
| Memory (RAM)    | 4 - 8 GB         | 16 - 32 GB |
| Storage      | 3 GB free space    | 6 GB |
|Network       | LAN or Localhost   | LAN or bridge adapter with wireshark capture |

</div>


## Software Reauirements

- **Python 3.x**.
- **PyCryptodome** → AES, RSA, hashing.
- **socket / hashlib** → networking + hash functions.
- **Wireshark** → traffic visualization.
- **mitmproxy** → proxy interception.
- **Tkinter (optional)** → GUI for chat.

### Installation Guide
In order to install the project on your device, follow the instructions bellow:
```bash
git clone <repository-url>
cd project-folder
python -m venv venv
venv\Scripts\activate        # (Windows)
source venv/bin/activate     # (Linux/macOS)
pip install -r requirements.txt

