---
title: Build


---

When you are ready to build your app, you press the **Build** button in the Phonegap Build Area section. Make sure you have [created and configured your `config.xml` file](/ide/tools/phonegap/config).

You should have set up your code signing keys in your Phonegap:Build account (more on keys below) and you should select which keys you wish to use for each platform you defined in your `<gap:platforms>` tag in the `config.xml` file.

Keys are configured from the **Account > Edit Setting > Signing Keys** tab in your Phonegap:Build account.

<img alt="Build settings" src="/img/buildsettings.png" class="simple"/>


## A bit about Keys

Phonegap has very good documentation on how to generate your keys as well as how to configure your Phonegap:Build account.

- [Android](http://docs.phonegap.com/phonegap-build/signing/android/)
- [iOS](http://docs.phonegap.com/phonegap-build/signing/ios/)

*Note If you do not see anything in the `Keys` area, review your `<gap:platforms>` content in the config.xml file*

# Android
To build and test, you don't need to do anything. You can leave the field empty . If you want to deploy a codesigned App, (which you will need to deploy via Google Play) then you need to generate a proper Certificate.

# iOS
Apple requires both a Codesigning Certificate and a Mobile Provisioning Profile. You need different ones for development and for App Store deployment.

# Windows
Windows does not require any certificates to build.


## Build Settings

# Private Application

Depending on the Phonegap:Build account plan you have, you can build a number of private applications. Check this box if you want to build as a private application. See [here](https://build.phonegap.com/plans) for more information on Phonegap:Build plans

# Enable Debug

Checking this box enables Phonegap Build debugging to allow you to use standard Web Inspector tools available from the PhoneGap Build site to debug PhoneGap apps while they are running on your device.

For more information on this see [Remote Debugging Tools](http://docs.phonegap.com/references/developer-app/debugging/)

# Enable Hydrates

Checking this box enables Phonegap:Build Hydration. Hydration is a tool that has two main benefits:

- Compilation times are improved significantly.
- Updates are pushed directly to the application installed on a device.

For more information on this see [Hydration](http://docs.phonegap.com/phonegap-build/tools/hydration/)

## Initiate Build
When you have selected keys and any settings, simply press the Build button. Codio now passes all information through to the Phonegap:Build platform, where the build is run in the background.

If the status does not complete in a reasonable time, you can do one of the following

- go to your Phonegap:Build account and click the main Apps tab, where you should see your app and its status
- check the status of the Phonegap:Build service [here](http://status.build.phonegap.com/)

## Download your App
When the build is completed you can deploy the app to your device in the following ways.

- download the native file and manually upload to your device
- scan the QR code to download from Phonegap:Build to your device

<img alt="Build" src="/img/build.png" class="simple"/>

