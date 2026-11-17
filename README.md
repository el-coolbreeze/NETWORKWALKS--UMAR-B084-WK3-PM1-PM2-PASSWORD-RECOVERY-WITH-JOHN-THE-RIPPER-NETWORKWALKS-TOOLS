# NETWORKWALKS--UMAR-B084-WK3-PM1-PM2-PASSWORD-RECOVERY-WITH-JOHN-THE-RIPPER-NETWORKWALKS-TOOLS
# Week 3 – Password Cracking with John the Ripper and Networkwalks Tools

## Cybersecurity Internship | NETWORKWALKS

This repository documents my Week 3 practical activities as a Cybersecurity Intern at **NETWORKWALKS**. The focus was **password recovery and password-strength testing** using John the Ripper (JTR), its graphical interface Johnny, and two browser-based Networkwalks tools.

The exercises involved working with the supplied password-protected PDF lab file, extracting its PDF hash, and using password-cracking tools to attempt to recover the password and open the PDF.

> **Ethical-use note:** These activities were performed as part of an authorised training exercise using supplied lab files. Password-recovery tools should only be used on files and systems you own or have explicit permission to test.

## Project objectives

- Understand the basic workflow involved in recovering a password from a protected PDF.
- Extract a PDF hash for use in a password-cracking tool.
- Use John the Ripper and Johnny GUI for a password-recovery exercise.
- Use Networkwalks Hash Calculator to extract a PDF hash.
- Use Networkwalks Password Cracker to attempt recovery from the extracted hash.
- Understand why password length, complexity, and uniqueness matter.

## Tools and resources

| Tool | Purpose |
|---|---|
| **John the Ripper (John)** | Password-auditing and recovery tool used to test password strength and recover passwords from supported hash formats. |
| **Johnny GUI** | Graphical interface for John the Ripper, allowing the lab workflow to be performed through a point-and-click interface. |
| **Networkwalks Hash Calculator** | Browser-based tool used to extract the hash from the supplied password-protected PDF. |
| **Networkwalks Password Cracker** | Browser-based tool used to attempt password recovery from the extracted PDF hash. |
| **Web browser** | Used to access the Networkwalks online tools. |
| **Windows PC / Kali Linux** | Lab environment. The project guide notes that John the Ripper is available in Kali Linux and that the Networkwalks browser tools can also be used from Kali. |

## Project Module 1 – Password Cracking with John the Ripper (JTR)

### Overview

The first module required recovering the password of the supplied protected PDF file, `My Locked PDF1.pdf`, using John the Ripper and its graphical interface, Johnny, on a Windows PC.

### Workflow

1. Downloaded and installed John the Ripper.
2. Downloaded and installed the Johnny graphical interface.
3. Configured Johnny to use the `john.exe` executable from John the Ripper's `run` folder.
4. Used a PDF hash-extraction tool to obtain the hash from the supplied protected PDF.
5. Copied the complete hash (beginning with `$pdf$`) into a text file named `hash1.txt`.
6. Opened the hash file in Johnny.
7. Started a new password-recovery attack and allowed the tool to process the hash.
8. Used the recovered password to open the supplied PDF and confirm that it was accessible.

### Key learning points

- John the Ripper can work with supported password-hash formats to audit password strength and recover passwords.
- Johnny provides a graphical way to load a password file and start an attack.
- The extracted hash must be complete and in the expected format for the tool to process it.
- Recovery time depends on factors such as password complexity and available computing resources.

**Evidence:** Add your own screenshots in `evidence/jtr/` and link them below.

- `evidence/jtr/01-johnny-configuration.png`
- `evidence/jtr/02-pdf-hash-extraction.png`
- `evidence/jtr/03-hash-file-loaded.png`
- `evidence/jtr/04-johnny-attack-results.png`
- `evidence/jtr/05-pdf-opened.png`

## Project Module 2 – Password Cracking with Networkwalks Tools

### Overview

The second module used two browser-based tools provided by NETWORKWALKS:

- **Hash Calculator:** https://networkwalks.com/hash-calculator/
- **Password Cracker:** https://networkwalks.com/password-cracker/

The objective was to extract the hash from the supplied protected PDF and submit that hash to the Password Cracker to attempt to recover the PDF password.

### Workflow

1. Downloaded the supplied protected PDF, `My Locked PDF1.pdf`, from the Networkwalks project task page.
2. Opened the Networkwalks Hash Calculator in a web browser.
3. Uploaded the protected PDF to extract its hash.
4. Copied the complete hash value, ensuring it began with `$pdf$`.
5. Opened the Networkwalks Password Cracker.
6. Pasted the extracted hash into the Password Cracker and started the attack.
7. Waited for the tool to complete and display the recovered password.
8. Entered the recovered password to open the supplied PDF and verify the result.

### Key learning points

- The hash-extraction and password-recovery stages are separate steps in the workflow.
- The complete hash must be copied accurately.
- Password-recovery time can vary depending on the password's simplicity or complexity.
- Browser-based tools can make a practical password-auditing exercise accessible without installing a desktop cracking application.

**Evidence:** Add your own screenshots in `evidence/networkwalks-tools/` and link them below.

- `evidence/networkwalks-tools/01-hash-calculator.png`
- `evidence/networkwalks-tools/02-extracted-pdf-hash.png`
- `evidence/networkwalks-tools/03-password-cracker-input.png`
- `evidence/networkwalks-tools/04-password-cracker-result.png`
- `evidence/networkwalks-tools/05-pdf-opened.png`

## What I learned in Week 3

This week's exercises gave me practical exposure to password auditing and recovery workflows. I learned how to:

- Extract a PDF hash and prepare it for a compatible password-cracking tool.
- Use John the Ripper through the Johnny graphical interface.
- Use Networkwalks Hash Calculator and Password Cracker in a browser.
- Follow a password-recovery workflow from hash extraction through to verification by opening the PDF.
- Appreciate the importance of strong, unique passwords in protecting sensitive documents.

The hands-on exercises were especially interesting because I could see how the tools worked with the extracted hash and how password complexity can affect the time required for recovery.

## Security takeaways

- Use long, unique passwords rather than short or commonly used passwords.
- Consider a reputable password manager to generate and store strong passwords.
- Protect sensitive documents with appropriately strong passwords.
- Avoid reusing passwords across accounts or documents.
- Only perform password-recovery or password-auditing activities where you have clear authorisation.

## Suggested repository structure

```text
Week-3-Password-Cracking/
├── README.md
├── evidence/
│   ├── jtr/
│   │   ├── 01-johnny-configuration.png
│   │   ├── 02-pdf-hash-extraction.png
│   │   ├── 03-hash-file-loaded.png
│   │   ├── 04-johnny-attack-results.png
│   │   └── 05-pdf-opened.png
│   └── networkwalks-tools/
│       ├── 01-hash-calculator.png
│       ├── 02-extracted-pdf-hash.png
│       ├── 03-password-cracker-input.png
│       ├── 04-password-cracker-result.png
│       └── 05-pdf-opened.png
└── project-guides/
    ├── W3-PM1-JTR.pdf
    └── W3-PM2-Networkwalks-Tools.pdf
```

*Only include project guides, screenshots, and other materials that you are permitted to share. Do not upload recovered passwords, live password hashes, private documents, or other sensitive information to a public repository.*

## Conclusion

Week 3 was an enjoyable and valuable part of my cybersecurity internship at **NETWORKWALKS**. Working with John the Ripper, Johnny GUI, and the Networkwalks Hash Calculator and Password Cracker helped me understand the practical steps involved in password auditing and why strong passwords are essential for protecting information.

I look forward to building on these skills and continuing to develop my knowledge of cybersecurity.

---

**Disclaimer:** This repository is for educational and documentation purposes. The activities described were carried out as part of an authorised training lab using supplied sample files. Do not use password-cracking tools against files, accounts, or systems without permission.

