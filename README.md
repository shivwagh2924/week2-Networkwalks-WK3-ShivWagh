
# 🔐 NETWORKWALKS | WEEK 3 – PASSWORD CRACKING

### Cybersecurity Internship – Batch B084

**Intern:** Aryan Govekar 
**Week:** 03  
**Project Modules:** PM1 & PM2  
**Topic:** PDF Password Cracking using John the Ripper and Networkwalks Tools

---

## 📌 Project Overview

This repository contains the practical implementation of Week 3, Project Modules 1 and 2, completed as part of the **Networkwalks Cybersecurity Internship (Batch B084)**.

The objective of this project was to recover the password of a password-protected PDF file (`My Locked PDF1.pdf`) using two different password-cracking approaches:

1. **John the Ripper (JTR) and Johnny GUI**
2. **Networkwalks Hash Calculator and Password Cracker**

Both methods demonstrate how password hashes can be extracted and tested against dictionary-based password attacks.

---

# 🛠️ WK3-PM1: Password Cracking Using John the Ripper

### 🎯 Objective
To extract the password hash of a protected PDF and recover its password using John the Ripper (JTR) and its graphical interface, Johnny.

### 🔧 Tools Used
- John the Ripper (JTR)
- Johnny GUI
- Online HashCrack PDF Hash Extractor
- Password-protected PDF file

### ⚙️ Steps Performed

**Step 1: Extract PDF Hash**

Uploaded the protected PDF to the Online HashCrack PDF Hash Extractor and generated its password hash in `$pdf$...` format.

The extracted hash was saved in a file named `hash1.txt`.

📸 **Screenshot:**

![Hash Extraction](screenshots/PM1/Hash-Extract.png)

**Step 2: Configure Johnny**

Opened Johnny, the graphical interface of John the Ripper, configured the John executable path, and loaded `hash1.txt` using the Open Password File option.

📸 **Screenshot:**


![Johnny Configuration](screenshots/PM1/JTR-PM1-Setup.png)
**Step 3: Perform Password Cracking**

Started the password-cracking process using Johnny.

The tool successfully recovered the password.

<details>
<summary>🔑 View Cracked Password</summary>

**Recovered Password:** `good-luck`

**Result:** 1 password cracked (100%).

</details>

📸 **Screenshot:**

![JTR Password Cracking Result](screenshots/PM1/JTR-PM1.png)

**Step 4: Verify the Password**

Opened the protected PDF using the recovered password to confirm that the password-cracking process was successful.

📸 **Screenshot:**

![Unlocked PDF](screenshots/PM1/W3-PM1-file-unlocked.png)

### ✅ PM1 Result

Successfully recovered and verified the PDF password using John the Ripper and Johnny GUI.

---

# 🌐 WK3-PM2: Password Cracking Using Networkwalks Tools

### 🎯 Objective
To recover the password of the same protected PDF using Networkwalks' browser-based Hash Calculator and Password Cracker.

### 🔧 Tools Used
- Networkwalks Hash Calculator
- Networkwalks Password Cracker
- Web Browser
- Password-protected PDF file

### ⚙️ Steps Performed

**Step 1: Generate PDF Hash**

Uploaded the protected PDF to the Networkwalks Hash Calculator.

The tool extracted the PDF password hash in `$pdf$...` format.

📸 **Screenshot:**

![Hash Calculator](screenshots/PM2/Hash-Calculator.png)

**Step 2: Perform Dictionary Attack**

Copied the extracted hash and pasted it into the Networkwalks Password Cracker.

Selected the dictionary attack method and started the cracking process.

The tool successfully recovered the password.

<details>
<summary>🔑 View Cracked Password</summary>

**Recovered Password:** `password1`

</details>

📸 **Screenshot:**

![Password Cracker Result](screenshots/PM2/Cracked.png)

**Step 3: Verify the Password**

Used the recovered password to open the protected PDF and confirmed that the file was successfully unlocked.

📸 **Screenshot:**

![Unlocked PDF](screenshots/PM2/W3-PM2-File-Unlocked.png)

### ✅ PM2 Result

Successfully recovered and verified the PDF password using the Networkwalks online password-cracking tools.



# 📊 Comparison: PM1 vs PM2

| Feature | PM1 – JTR | PM2 – Networkwalks |
|---|---|---|
| Tools | John the Ripper & Johnny | Networkwalks Online Tools |
| Interface | Desktop GUI | Web-based |
| Hash Extraction | Online HashCrack | Hash Calculator |
| Attack Method | Password cracking | Dictionary attack |
| Installation | Required | Not required |
| Recovered Password | `good-luck` | `password1` |

---

# 💡 Key Learnings

Through these practical exercises, I learned:

- How to extract password hashes from protected PDF files.
- How PDF password hashes are represented in `$pdf$...` format.
- How to configure and use John the Ripper with Johnny GUI.
- How to perform dictionary-based password attacks.
- How to use browser-based password-cracking tools.
- How to verify recovered passwords by opening protected files.
- Why short and predictable passwords are vulnerable to dictionary attacks.

### 🔐 Security Takeaway

Weak and predictable passwords can be recovered quickly using publicly available password-cracking tools.

Using long, unique, and complex passwords helps improve security and reduces the risk of unauthorized access.


### ⚠️ Disclaimer

This project was conducted strictly for educational and cybersecurity training purposes as part of the Networkwalks Cybersecurity Internship.

The target PDF and associated lab materials were provided by Networkwalks. Password recovery was performed only on the authorized training file.

**For educational purposes only. Always obtain proper authorization before conducting password recovery or security testing.**

---

⭐ If you find this project useful, feel free to explore the repository!
