# 🔐 VigenereCipher

**Python implementation of the Vigenère cipher** using a custom alphabet: **A-Z + 0-9**.  
The project supports **encryption, decryption, simple automatic key guessing, frequency analysis, and comparison of ciphertext statistics for different key lengths**.

📄 **Versions:** `maineng.py` (English), `mainpl.py` (Polish)  
📊 **Outputs:** generated `.txt` files with encrypted / decrypted text and printed frequency analysis in the console

---

## 🎯 Goal
This project focuses on:
- implementing the **Vigenère cipher** with a custom alphabet,
- encrypting and decrypting text files,
- preserving spaces, punctuation, and line breaks without consuming key characters,
- analyzing **character and word frequency** before and after transformation,
- comparing how ciphertext statistics change for key lengths:
  - **3**
  - **6**
  - **9**
  - **12**
  - **16**

---

## 🧠 Cipher rules
### 🔹 Alphabet
The cipher works on the following alphabet:

```text
ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789
```

### 🔹 Encryption / Decryption

For every character belonging to the alphabet:

* encryption shifts the symbol forward according to the matching key character,

* decryption shifts it backward using the same key.

### 🔹 Non-alphabet characters

Characters such as:

* spaces,

* punctuation,

* line breaks,

* other symbols

are copied without modification and do not consume key characters.

---
## ⚙️ Features

* file-based encryption
* file-based decryption
* simple automatic key guessing mode
* frequency analysis of:
  * letters/digits
  * words

* comparison of:
  * 3 most common letters/digits
  * 3 least common letters/digits
  * 3 most common words
  * 3 least common words

* comparison mode for key lengths:
  * 3 / 6 / 9 / 12 / 16

* support for:
  * user-defined keys
  * keys generated from pattern zaq1@WSX

---
## 📂 Repository structure
```
.
├─ maineng.py
├─ mainpl.py
├─ LICENSE
└─ .gitignore
```

---
## ▶️ Running the project
No external libraries are required.
### Run with Python 3:
* English version  
```python maineng.py```  
* Polish version  
```python mainpl.py```

---
## 🖥️ Available modes
### English version (maineng.py)
e — encrypt  
d — decrypt  
a — automatic breaking without key  
p — compare frequencies for key lengths `3, 6, 9, 12, 16`  

### Polish version (mainpl.py)
s — szyfrowanie
d — deszyfrowanie
a — automatyczne łamanie bez hasła
p — porównanie częstotliwości dla długości hasła `3, 6, 9, 12, 16`

---
✨ Analysis output

The program can analyze text before and after encryption / decryption.

It shows:

3 most common letters/digits

3 least common letters/digits

3 most common words

3 least common words

This makes it useful not only for cipher operations, but also for demonstrating how encryption changes text distribution.

---

📊 Key length comparison

The project includes a comparison mode for the following key lengths:

3

6

9

12

16

Keys can be:

entered manually by the user,

or generated from the pattern:

zaq1@WSX

After filtering to the project alphabet, the pattern becomes:

ZAQ1WSX

---

🧪 Automatic key guessing

The repository also includes a simple heuristic-based automatic key guessing mode.

⚠️ Important note:
this mode is experimental and intended mainly for educational purposes.
It may work on some inputs, but it does not guarantee correct recovery of the original key, especially for:

short texts,

difficult ciphertexts,

texts with unusual symbol distributions.

---

🖼️ Quick preview
Example workflow

Read text from file

Encrypt or decrypt with Vigenère cipher

Save result to output file

Compare text statistics before and after transformation

Frequency analysis includes

top 3 most common letters/digits

top 3 least common letters/digits

top 3 most common words

top 3 least common words

Comparison mode

The project can automatically generate and compare ciphertexts for different key lengths to observe how character distribution changes.

---

💡 Educational purpose

This project is useful for:

learning how the Vigenère cipher works,

understanding how classical encryption changes frequency distribution,

comparing ciphertext structure for different key lengths,

demonstrating basic cryptographic analysis in Python.

---

### 🧑‍💻 Author

Created by Avuii
