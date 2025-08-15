# Office Deployment Tool

This repository contains a `configuration.xml` file used with the Office Deployment Tool (ODT) to perform a customized installation of Microsoft Office.

The configuration file is designed to install only Word, Excel, and PowerPoint, excluding other apps to optimize disk space and system performance. It installs the 64-bit version, uses the Monthly Enterprise update channel, and the Product ID `O365ProPlusRetail` for proper licensing.

---

## How to use

1. Download the Office Deployment Tool from Microsoft's official site:
   [https://www.microsoft.com/en-us/download/details.aspx?id=49117](https://www.microsoft.com/en-us/download/details.aspx?id=49117)

2. Extract `setup.exe` and place it in the same folder as `configuration.xml`.

3. Open a command prompt as Administrator and navigate to the folder where both files are located. For example:

   ```
   cd C:\ODT
   ```

4. Run the installation command:

   ```
   setup.exe /configure configuration.xml
   ```

This will start the installation with the custom settings defined in the configuration file.

---

## Configuration file overview
* **Product ID**: Defines which Office suite to install (`O365ProPlusRetail`).
* **OfficeClientEdition**: Installs the 64-bit version of Office.
* **Channel**: Sets the update channel (Monthly Enterprise) for Office updates.
* **Language**: Specifies the language of the Office installation.
* **Excluded Apps**: Lists Office apps to exclude from installation (e.g., Outlook, Teams, OneNote).
* **Display Level**: Controls the installer UI (set to show progress).
* **Auto Activate**: Automatically activates Office after installation.
