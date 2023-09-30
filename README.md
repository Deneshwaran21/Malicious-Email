# Malicious-Email
Investigating a Malicious Email using Maltego

# 1.Prerequisites
**Setup Overview**
    While working with Ethical Hacking approaches, we should ensure that the tools we use, are properly installed and configured as per our requirements. To seamlessly and safely perform the hands-on during the workshop, we will be using the Kali Linux Command line version.
    
# 2.Setting Up WSL2 in your Windows System
    - Firstly, [**update your windows](https://support.microsoft.com/en-us/windows/get-the-latest-windows-update-7d20e88c-0568-483a-37bc-c3885390d212#:~:text=To%20check%20for%20updates%2C%20select,can%20choose%20to%20install%20them.&text=If%20you%20run%20into%20problems,at%20Troubleshoot%20problems%20updating%20Windows.).**
    - To install the Windows Subsystem for Linux (WSL) feature in your Windows, you can click on [**this link**](https://learning.ccbp.in/installations/ide-setup-instructions) for the step-by-step installation process.

💡 **Kali Linux: Overview**

- Kali Linux (or simply, “Kali”) is a Debian-based Linux distribution aimed at advanced Penetration Testing and Security Auditing
- It is built for Security professionals, IT administrators, and practitioners alike, enabling them to conduct advanced Penetration Testing, Forensic Analysis, Security Auditing, and much more.
- Kali Linux comes up with several hundred tools that are geared toward various information security tasks, such as Penetration Testing, Security research, Computer Forensics, and Reverse Engineering.

Also, Windows Subsystem for Linux (WSL) has [two different versions](https://docs.microsoft.com/en-us/windows/wsl/compare-versions), “WSL 1” and “WSL 2”. **WSL 2 is the preferred** and default option when installing WSL.

-After setting up the WSL environment, you can open the Command line / Windows Power Shell as an administrator and type the following command. (wsl --update)
-To install Kali-Linux, enter the command below in the Power Shell and run it. (wsl --install --distribution kali-linux)
-Upon completion, you would be asked to enter the username and password that you would want to set for Kali Linux. You can choose to have both the username and password as “kali”. 
Note: The password will not be visible to you when you type it.
-After entering the password, it asks you to re-type the password for verification.
After this, the Kali-Linux environment will open in the same terminal indicated by the change in the command prompt color and the title of the window as shown below. 
![image](https://github.com/Deneshwaran21/Malicious-Email/assets/139675815/5bb8a832-fdea-4ef0-9aaf-cd7b8abca482)
With this, the Kali-WSL will be installed successfully.
After everything has been set up and installed, you can run Kali from the Windows Start menu.

# 3.Installing Win-Kex
💡 **Overview:**

- Win-kex gives a GUI desktop experience for Kali-Linux in WSL2.
- You can install and set up Win-Kex in your system either by following the steps mentioned below or referring to [**Kali’s official documentation**](https://www.kali.org/docs/wsl/win-kex/)
- When using Kali for the first time or when installing something in our Kali Linux, it is a good practice to run the apt-*update* command.
    
    Run the following command to update the Kali-Linux repositories: sudo apt update
  Note that when running super user commands (sudo), you will be prompted for the password. You can enter the password that you configured earlier (Kali).
Note: The password will not be visible to you when you type it. 
Next, to install Win-Kex via the Kali Linux command line, run the following command: sudo apt install -y kali-win-kex
Now to start Win-Kex in windowed mode, run this command: kex --win -s
You will be prompted for a new password again for Win-Kex which should consist minimum of 6 characters.
![image](https://github.com/Deneshwaran21/Malicious-Email/assets/139675815/f7f964b1-cb4f-4e7c-891a-bd20687a496f)

1. Provide a password that is 6 characters or above and press Enter. Then verify the same by retyping and pressing Enter.
2. Type “y” for the question.
3. You need to type the same password again and verify it as it is the first time using Win-kex.
4. Finally, type the Kali-Linux password and press enter. 

Once done, you should have the Kali Linux’s Win-Kex window opened in full-screen mode and looking something like this:
![image](https://github.com/Deneshwaran21/Malicious-Email/assets/139675815/9ed54e6a-ee3c-4cf0-9808-96dba488a03b)

💡 **Note:**

- Press F8 and uncheck the “Full-Screen” checkbox to change from Full screen to windowed mode.
- Also, note that the Windows taskbar will hide some portion of the Kali-Linux window.
- You can close all the unnecessary notifications that pop up after the Kali Linux gets opened.

These are the primary steps to be followed to install and run kali Linux in your system.
For futhur more information on creating this project refer [Youtube](https://www.youtube.com/watch?v=a2ZvpwF3u-M&pp=ygUWaG93IG1hbHRlZ28gdG9vbCB1c2VkIA%3D%3D) 

    
