# passkey

- Register the the target devices' UDID on Apple Developer portal
- Select `Generic iOS Device`
- In your xcode project go to **Product > Archive**
- Distribute as Ad Hoc Deployment
- Copy the generated `ipa` file and `manifest.plist` file to `static` folder
- Update the `href` of the anchor link to `itms-services://?action=download-manifest&url=https://passkey-web.netlify.com/manifest.plist`
- The app should start installing on any registered device that clicks on that link.
