# Office Deployment Tool

This `configuration.xml` file is set up to install only Word, Excel, and PowerPoint using the Office Deployment Tool.
I created it to avoid installing apps I don’t need, like Outlook, Teams, or OneNote.

It installs the 64-bit version, uses the Monthly Enterprise update channel, and the Product ID `O365ProPlusRetail`.

To install, just run:

```
setup.exe /configure configuration.xml
```
