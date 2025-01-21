# **DualKey - Seedphrase Encryption/Decryption Tool**

![DualKey](https://img.shields.io/badge/Python-3.11-blue) ![License](https://img.shields.io/badge/license-MIT-green)

**DualKey** is a simple command-line tool for encrypting and decrypting sensitive text, such as seed phrases, using a user-defined encryption key and offset.

---

## **Features**

- ✅ Encrypts text using a custom encryption key and offset  
- ✅ Decrypts encrypted text back to its original form  
- ✅ Simple command-line interface with input validation  
- ✅ ANSI color formatting for better readability  
- ✅ Cross-platform support (Linux, macOS, Windows)  

---

## **Installation**

### **Using Python (Recommended)**

Ensure you have **Python 3.11+** installed, then install the tool using `pip`:

```bash
pip install dualkey
```

Using Homebrew

```bash
brew install dualkey
```

## Usage

1. Running the tool
After installation, run the following command:

```bash
dualkey
```

You will be prompted to enter an encryption key and offset.

### 1. Encryption Example
```bash
Enter encryption key (4-digit number): 1234
Enter offset value (4 to 6 digit number): 56789
Do you want to (E)ncrypt or (D)ecrypt? E
Enter text to encrypt (max 300 characters): my seed phrase
```
Output:
```bash
Encrypted Text: 1422395 1693201 1452487 1347403 1347403 1358632 1508570 1463723 1422395 1324952 1452487 1422395 1463723 1441258 1399940
```

### 2. Decryption Example
```bash
Do you want to (E)ncrypt or (D)ecrypt? D
Enter the encrypted text to decrypt: 1422395 1693201 1452487 1347403 ...
Output:
```

```bash
Decrypted Text: my seed phrase
How It Works
The tool uses a simple formula to encrypt each character of the input:
```
```sql
Encrypted character = (ASCII value * key) - offset
To decrypt, it reverses the formula:
```
```java
Original ASCII = (Encrypted value + offset) // key
```

## 2. Example Use Cases

- Secure storage of cryptocurrency seed phrases
- Encrypting personal notes
- Quick encryption for sensitive data on the go
- Security Notice
  
**⚠ This tool does not provide cryptographic security.**
It is a simple educational utility and should not be used for high-security applications. Always rely on industry-standard encryption methods for sensitive data.

## 3. Development

Clone the repository
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/dualkey.git
cd dualkey
```

Install dependencies
```bash
pip install -r requirements.txt
```

Run the tool locally

```bash
python dualkey.py
```

## 4. Contributing

Contributions are welcome! To contribute:

- Fork the repository
- Create a feature branch (git checkout -b feature-name)
- Commit your changes (git commit -m 'Add feature')
- Push to your branch (git push origin feature-name)
- Create a Pull Request

## 5. License

This project is licensed under the MIT License. See the LICENSE file for details.

## 6. Contact
For questions, suggestions, or issues, feel free to open an issue on GitHub or reach out via email:

📧 denverhnt@gmail.com
🐙 GitHub: @ilovespectra