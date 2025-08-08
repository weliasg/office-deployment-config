# Microsoft 365 Custom Installation Settings

This repository contains a custom configuration file for installing Microsoft 365 using the [Office Deployment Tool (ODT)](https://www.microsoft.com/en-us/download/details.aspx?id=49117).

## What's Included

This setup installs a minimal version of Microsoft 365 (64-bit, Current Channel) with just the essentials.

### Included Apps:
- Word
- Excel

### Excluded Apps:
- Access  
- Outlook  
- PowerPoint  
- Publisher  
- OneNote  
- Teams  
- OneDrive  
- Skype for Business (Lync)

## Key Settings

- **Silent install**: No UI prompts during installation  
- **EULA**: Automatically accepted  
- **Auto activation**: Enabled  
- **Device-based licensing**: Disabled

## How to Use

1. [Download the Office Deployment Tool (ODT)](https://www.microsoft.com/en-us/download/details.aspx?id=49117)
2. Place `Configuration.xml` in the same folder as `setup.exe` (from the ODT download)
3. Open Command Prompt and run:

   ```bash
   setup.exe /configure Configuration.xml
