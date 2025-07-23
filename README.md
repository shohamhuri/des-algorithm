בהחלט! הנה תוכן מלא של קובץ `README.md` שתוכלי להעתיק ולהדביק לרפוזיטורי שלך:
# python-des

Manual implementation of the DES encryption algorithm in Python, including both encryption and decryption.

## 🔐 Overview

This project provides a low-level implementation of the **Data Encryption Standard (DES)** in Python. It demonstrates all major steps of the algorithm, including permutations, key scheduling, expansion, S-box substitution, and XOR operations — all without using any external libraries.

## 🧠 How It Works

1. **Input**:  
   - 16-character hexadecimal plaintext  
   - 16-character hexadecimal key

2. **Key Generation**:
   - Initial permutation (PC-1) reduces key to 56 bits  
   - Key is split and left-shifted for 16 rounds  
   - Each round key is compressed to 48 bits using PC-2

3. **Encryption**:
   - Initial permutation on the plaintext  
   - 16 rounds using Feistel structure  
   - Expansion, XOR with round key, S-box substitution, permutation  
   - Swap halves and final permutation

4. **Decryption**:
   - Same process as encryption, with round keys in reverse order

## ▶️ Usage

Run the script:


python des.py

Example input:

Which string do you want to encrypt? 123456ABCD132536
What is your key? AABB09182736CCDD

## 📁 File

* `des.py` – Main script containing the full DES implementation

## 📚 References

* [Wikipedia - Data Encryption Standard](https://en.wikipedia.org/wiki/Data_Encryption_Standard)
* S-boxes, permutation tables, and key schedule follow the original DES specification

## ✍️ Author

Shoham Huri
