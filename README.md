# What Does This "Key"logger Do? 🤔
* First 10 seconds you get **System Information, Local and Public IP Information, Local Users Information, OS Information** and **Wifi passwords** from target computer and send to your mail.

* 2nd and other mails (every 10 seconds) you get **Keyboard Inputs**, **Mouse Coordinates**, **ScreenShot**, **Microphone Recording** and **Photo (if target has a WebCam)** from target computer and send to your mail.

* If the target finds the code and opens the file, the program **Deletes** itself.

* The objective of this repository is to serve as an example, it has educational purposes, and in no case does it pretend to be perfect or fully functional.

# INSTALLATION
```bash
pip install -r requirements.txt
```

# About Getting Credentials

* ***Windows OS*** saves **Web Credentials** and **Windows Credentials** in the **Credential Manager.**

* However, the program may encounter some errors while decoding user passwords.

* If some passwords are still not decoded, you can decode them with the `decode.py` (at least some of them).

* Please note that is not possible anyway retrieve or save user passwords in hashed or plaintext form using methods provided by the Windows API or other legal means.

* User passwords are sensitive information and are handled with the highest level of security.

# ⚠️ Warning ⚠️

* You need to run the script as administrator because the script copies itself to `C:\Windows\System32`

* Also, remember that **even the higher-level** file copying functions like `shutil.copy()` and `shutil.copy2()` can't copy all file metadata.

* On Windows, file owners, Access Control Lists (ACLs) and alternate data streams are not copied.

# USAGE 🐣

* Create an account on https://mailtrap.io/ to use a temp mail.

* Click on ***Show Credentials*** to see your **Username** and **Password.**

![image](https://github.com/darkbytehunter/Keylogger/blob/main/images/Access%20Token.jpeg)

* After clicking on ***Show Credentials*** set your own **SMTP Username** and **SMTP Password** on `keylogger.py`

![image](https://github.com/darkbytehunter/Keylogger/blob/main/images/Show%20Credentials.jpeg)

* Then create an account on https://ipinfo.io/ to get your **Access Token.**

![image](https://github.com/darkbytehunter/Keylogger/blob/main/images/Username%20and%20Password.jpeg)

* After you have set up the token in your ipinfo account, you are done! ✔
