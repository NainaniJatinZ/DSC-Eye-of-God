<h1 align="center">Eye of God</h1>

<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1JVGHzA8G-WLSilfG0LtHMJudbn2_Yfxs"> 
</div>

<br>

[![](https://img.shields.io/badge/Made_with-Flutter-green?style=for-the-badge&logo=flutter)](https://flutter.dev/)
[![](https://img.shields.io/badge/Made_with-Google%20Maps%20Platform-green?style=for-the-badge&logo=google-maps)](https://developers.google.com/maps/documentation)
[![](https://img.shields.io/badge/Made_with-dart-green?style=for-the-badge&logo=dart)](https://dart.dev/)
[![](https://img.shields.io/badge/C++-CPP-green.svg?style=for-the-badge&logo=c%2B%2B)]()
[![](https://img.shields.io/badge/Made_with-Opencv-green?style=for-the-badge&logo=opencv)](https://opencv.org)
[![](https://img.shields.io/badge/Made_with-Tensorflow-green?style=for-the-badge&logo=tensorflow)](https://www.tensorflow.org)
[![](https://img.shields.io/badge/Made_with-Google_Cloud-green?style=for-the-badge&logo=google-cloud)](https://cloud.google.com)
[![](https://img.shields.io/badge/Made_with-Keras-green?style=for-the-badge&logo=keras)](https://keras.io)
[![](https://img.shields.io/badge/Made_with-Arduino-green?style=for-the-badge&logo=arduino)](https://www.arduino.cc)
</br>

</div>



---
<h2><strong>About</h2></strong>
<p>
The World Health Organization puts the global figure of visually-impaired and blind people at 285 million. For these people, navigating busy urban landscapes can be extremely challenging.  
To offer a solution to the urban-dwelling visually-impaired, we built “Eye of God”. It is an easy-to-use navigation system for visually impaired people, acting as their “virtual-cane” to help them navigate to their destination all by themselves without needing the assistance of other people.  
<p>
One reason why blind people typically stay close to home is because they sense the world is not made for them. It would be really wonderful for blind people to feel they can visit new places on their own, and for them to be able to say, 'I can walk through malls or venues without this sense of hopelessness or of missing information.'  
</p>
<p>The Eye of God navigation system comes in two modes: Indoor Navigation and Outdoor Navigation. </p>

<p><strong>Indoor Navigation:</strong> The user is prompted to speak out a destination like “General Ward Sign” in a hospital. Once the system recognises the said text in the vicinity, a pulsating vibration will be given on the motor of the belt which is in the direction of the destination. For all the other objects in the frame, a constant vibration will be produced on detection, to avoid deviation from the path.
</p>
<p><strong>Outdoor Navigation:</strong> The user is prompted to speak out the destination, and the most optimal route is calculated. Since blind people are more efficient in hearing and possess stronger perception than normal people, therefore the system is focused on alerting the user through vibration (Haptic) and voice feedback. Step by step sound-based navigation commands are provided along with alerting the user about obstacles in the path through vibration from four motors mounted on a waist belt. Two pulses followed by constant vibration will be provided for pre-determined dangerous objects. When the user needs to make a turn, the system also provides the exact measure (in degrees) of the turn along with pulsating haptic feedback through leftmost or the right most motor depending upon the turn to inform the user the correct direction to turn to, to ensure user stays on route.  
This innovative use of technology can help visually impaired people feel more empowered and independent, thus bridging the gap and getting them at par with the sighted ones.  
</p>
<strong>In accordance with</strong>: 

* United Nations' Sustainable Development Goal 10: Reduced Inequalities. 

* United Nations' Sustainable Development Goal 9: Industry, Innovation, & Infrastructure.  

* United Nations' Sustainable Development Goal 16: Peace, Justice & Strong Institutions. 
<br>

---

<h2><strong>App Workflow</h2></strong>

* Outdoor Navigation
<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1Fm020SUF825Hw8lYa-mwOMQROmKdCcCP"> 
</div>
<br>

* Indoor Navigation
<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1puYMmGfSwPho6IkJVFx9F--ysxvZ9GGR"> 
</div>
<br>


<h2><strong>How to run</h2></strong>

<h3><strong>Flutter Project:<h3></strong>

`eye_of_god`

<h3><strong>ESP32 Code:<h3></strong>

Compile and execute the `ESP_Belt/ESP_Belt.ino` file on an ESP32 board with the necessary circuitary.

<h3><strong>OpenCV CPP Setup:</h3></strong>

1. Download OpenCV framework for iOS:https://docs.opencv.org/4.5.2/d5/da3/tutorial_ios_install.html
2. Copy or create symlinks:
	opencv2.framework to native_opencv/ios
3. Open Runner.xcworkspace and copy  OpenCV framework to Runnner(.xcproject) and Runner(.xcworkspace).

<h3><strong>Google Maps Setup:</h3></strong>

1. Paste Google Maps API Key ios/Runner/AppDelegate.swift:
	`GMSServices.provideAPIKey("YOUR-API-KEY")`

<h3><strong>Xcode Setup:</h3></strong>

1. Change the development team in Targets/Runner/Signing&Capabilities to your Apple ID.
2. Add a unique Bundle identifier

<h3><strong>Model Files:</h3></strong>

Incase the model files ("*.tflite") are missing from `eye_of_god/assets` folder, download it from here and place it in `eye_of_god/assets`:
https://drive.google.com/drive/folders/1UU3Cknl5Ns4tQJxeLE_aPkNXSMrRk8VF?usp=sharing


Run the app using `flutter run` in the main directory of the project `eye_of_god`.


---

<h2><strong>Circuit Diagram</h2></strong>
<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1RfGB6AxfB9v8Ie4y9r5t1Q-lGVsAGfDv"> 
</div>
<br>

---
<h3><strong> For Outdoor Navigation:<h3></strong>

1.	Turn on the belt for the app to pair automatically with it.
2.	Run the Flutter Application on your Phone and mount it to a VR headset.
3.	Press the button on the belt to activate speech input and dictate “Start Outdoor Navigation”.
4.	Dictate your destination starting with "Take me to \<your destination here>".
5.	Follow the commands dictated by the app and feedback from vibration motors to reach the destination.





<h3><strong>For Indoor Navigation:<h3></strong>

1.	Turn on the belt for the app to pair automatically with it.
2.	Run the Flutter Application on your Phone and mount it to a VR headset.
3.	Press the button on the belt to activate speech input and dictate "Start Indoor Navigation".
4.	Dictate the label of your destination starting with "Take me to \<destination label here>".
5.	Follow the pulsating motor to reach your destination.

---
<h2><strong>App Screenshots</strong>

* Outdoor Mode
<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1xR6G6FwNvBosXF4Mx8-pF525r7UkPTSe"> 
</div>

* Indoor Mode
<div align="center">
<img src="https://drive.google.com/uc?export=view&id=1V06ynztt7X0XkRibk-oEGH_AyV2VPp7n"> 
</div>

---
<h2>References</h2>


https://github.com/intel-isl/MiDaS

https://medium.com/flutter-community/integrating-c-library-in-a-flutter-app-using-dart-ffi-38a15e16bc14

https://stackoverflow.com/questions/62212942/how-to-use-opencv-with-dartffi-on-ios

https://medium.com/dartlang/dart-asynchronous-programming-isolates-and-event-loops-bffc3e296a6a

https://medium.com/@am15hg/real-time-object-detection-using-new-tensorflow-lite-flutter-support-ea41263e801d


<br>

---

<br>
Link to the Demo Video:
[Eye of God](https://youtu.be/zipQJU651U0)
<br>
---

<br>
	
<h3 align="center"><b>Developed by Team Hack Inversion</b></h3>

[![](https://img.shields.io/badge/LinkedIn-Anish_Pawar-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/anish-pawar-5300a9192/)

[![](https://img.shields.io/badge/LinkedIn-Gayatri_Patil-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/gayatri-patil-48316b203/)

[![](https://img.shields.io/badge/LinkedIn-Jatin_Nainani-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/jatin-nainani-a6b2331b3/)

[![](https://img.shields.io/badge/LinkedIn-Priyanka_Hotchandani-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/priyanka-hotchandani/)
