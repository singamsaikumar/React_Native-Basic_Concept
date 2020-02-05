
1) SOFTWARE TO INSTALL
     a) java
     b) android studio
     c) node

 2) Set the paths for 
    a) java sdk
        C:\Program Files\Java\jdk1.8.0_161
    b) android sdk
         C:\Users\SREEKANTH-PC\AppData\Local\Android\sdk  
    c) android sdk platform-tools
         C:\Users\SREEKANTH-PC\AppData\Local\Android\sdk\platform-tools
     d) node (it will create automatically)
     in environment variables, if not created automatically

3) In project in Android folder
    create local.properties file (.properties)  which contain android sdk path like this  
    sdk.dir = C:\\Users\\SREEKANTH-PC\\AppData\\Local\\Android\\Sdk

4) To Platform Install
    Open Android Studio and go to SDK manager(blue downarrow icon on top-right corner)
    download the  (check the checkbox Show pakckage Details)
      Android SDK Platform 26(any that u want)
   Google APIs Intel x86 Atom_64 System Image

5) For Emulator: 
    (make sure cpu virtual technology(something related to virtual) enabled (in boot panel))
    (make sure that in sdk manager in sdk tools intel emulator accelerator(HAXM installer) 
    installed)
    Go to AVD Manager(meroon red arrowdown icon)
    hit on create vertual device -- select the phone size(which phone size u want) and click next
    then download the android version image and  click next
    then select potrait mode and click finish


Commands Needed for Android:    

1) BUNDLE THE JS FILES AND CHECK FOR SYNTAX ERRORS IN ALL .js FILES:
  react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
  (not two lines just copy and past in notepad it will make it one line)

2) CLEAN THE ANDROID GRADLE:
     cd android           -  goes to android folder directory
     gradlew clean      -  clean the android gradle
     cd..                      -  back to directory

3) RUN THE REACT NATIVE CODE:
    react-native run-android 

4) TO INSTALL ALL DEPENDENCIES IN package.json FILE
     npm install

5) TO INSTALL PARTICULAR DEPENDENCY 
     npm instll --save react-native-drawer(this is name of dependency)--(downloads latest verson)

6) Ctrl+c and y+enter  to terminate batch job


Commands Needed for IOS:      

1) TO CEAN CACHE:
     sudo npm start -- -- reset-cache

2) TO CREATE BUILD FOLDER IN IOS FOLDER:
     react-native run-ios  

3) BEFORE RUNNING A PROJECT IN MAC MAKE SURE THAT COCOPAD INSTALLED  


Example error handling:

 1) In android folder-bundle.gradle 
     (if error in classpath, check here)
     classpath 'com.android.tools.build:gradle:3.1.2' 
     (make it  3.2.0 (may be latest))

2) In android folder-gradle-wrapper-gradle-wrapper.properties
    (if error in extracting gradle zip, check here)                         
    distributionUrl=https\://services.gradle.org/distributions/gradle-4.4-all.zip
    (make it 4.6 (may be latest))
