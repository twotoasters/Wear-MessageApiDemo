Wear-MessageApiDemo
===================

This is a sample Android project to demo the Wear MessageApi. It consists of two modules:
- **mobile** - The phone app
- **wear** - The Wear app

The mobile app is simply a Service (**ListenerService**) that listens for messages from the Wear device. When the mobile app gets a message, it displays it as a Toast.

The Wear app talks to the mobile app through the Android Wear MessageApi. It contains only an Activity (**MyActivity**) that contains a Button. When the user taps the Button, a message is sent to the mobile app indicating that a Toast should be shown.

**Note:** When deploying to your device, make sure you push the Wear app's apk to the Wear device and the mobile app's apk to the phone/tablet. If there's no signing going on (which there isn't by default), the Wear app won't be automatically pushed when you install the mobile app.