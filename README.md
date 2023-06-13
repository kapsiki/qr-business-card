# QR Business Card

This project contains source code and a basic HTML page to generate a business card embedded 100% inside of a QR code.  From a real world perspective, scanning the QR code simply brings up the native contact viewer on the smartphone which scanned the QR code, making it very easy to save the contact immediately or continue to edit the contact.  From a technical perspective, the QR code generated by this process embeds the source code for a VCF contact file which should be automatically interpreted by the receiving device.  The QR code generated from this process does not link to a website or other tracking service as many QR code services will do in order to share and display contact information.  

## Table of Contents
- [Contact Syntax](#contact-syntax)

## Contact Syntax

The following skeleton code represents the syntax and structure used for the contact creation.

```
BEGIN:VCARD
VERSION:3.0
N:{{Last name}};{{First name}};
FN: {{Full name}}
ORG:{{Organization}};
TEL;TYPE=mobile;TYPE=pref:{{Primary phone number}}
TEL;TYPE=home:{{Secondary phone number}}
EMAIL;TYPE=INTERNET;TYPE=WORK:{{Work email}}
EMAIL;TYPE=INTERNET;TYPE=HOME:{{Personal email}}
TITLE:{{Job title}}
URL:{{Primary website}}
URL:{{Secondary website}}
VERSION:3.0
END:VCARD
```
