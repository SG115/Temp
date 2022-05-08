# ENVIRONMENT SETUP 

## Arduino IDE Environment Setup
### Libraries Installation:
1. At Arduino IDE, go to menu Sketch -> Include Library -> Manage Libraries...
2. In Library Manager Window, search "firebase" in the search form then select "Firebase ESP8266 Client".
3. Click "Install" button.

For other help or issues, please refer : [Link](https://github.com/mobizt/Firebase-ESP8266)

### How to setup firebase in Arduino:
The only required things for our project is the firebase URL and API Key to connect the realtime firebase with NodeMCU.
1. <strong> Set your FIREBASE_HOST </strong> <br> <br>
  Open your Realtime Database and copy your Firebase host to in to your arduino code (FIREBASE_HOST).
  When your copy Firebase host, remove " https:// "and"/" from the Firebase host. <br> <br>
  #define FIREBASE_HOST "your FIREBASE HOST"
  
2. <strong> Set your FIREBASE_AUTH </strong> <br> <br>
  Open your Realtime Database and go to project overview > project settings > Service accounts > Database secrets and copy your Secret and paste in to your FIREBASE_AUTH.
  <br> <br> #define FIREBASE_AUTH "Your secret"
  
Please refer [this](https://create.arduino.cc/projecthub/pulasthi-Narada/connecting-esp8266-to-firebase-to-send-receive-data-4adf66) for the proper steps.

### Run the Arduino Code:
1. First upload the code by clicking Upload on the top-left side of Arduino IDE. This might take 2-3 minutes to write code in NodeMCU.
2. Now, activate the hardware by clicking Veriy aside Upload button. 
3. To see the real time changes, open the serial monitor on the top right side of Arduino IDE.

### Testing the Code:
1. Once you run the Arduino Code, you can now see the realtime changes by changing the garbage level inside the dustbin.
2. You can see the data gets realtime updates in serial monitor.
3. Since the Firebase is connected to NodeMCU, the realtime data changes will also be reflecting in the Firebase directly corresponding to particular bin.
4. Firebase is connected to Android Application, so you can see the realtime changes directly in the app.

## Android Studio Setup:
1. For Android Studio Installation, please refer [this](https://developer.android.com/studio/install) or [this](https://www.c-sharpcorner.com/article/how-to-download-and-install-android-studio-in-windows-10/).
2. Simply import the "App Code" folder in Android Studio. If new, see how to do it in [this](https://help.dropsource.com/docs/documentation/after-dropsource/accessing-your-source-code/importing-source-code-into-android-studio/#importing-into-android-studio).
3. Now, build and run the app on emulator or via USB debugging on your smartphone. Refer [this](https://developer.android.com/studio/run) to know how to do it.

