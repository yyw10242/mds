# Flutter

## PUB

Dart's Package manager like nuget, pip, etc.

 

### When you're using other's local project written in dart with package.

Used Dart Package installed with pub must be reclaimed.

1. If pub is not installed
   1. Terminal - flutter pub get
      VSCode - open pubspec.yaml - press ![image-20210201101956815](D:\KULS\DailyMD\2102\referenceImage\210221\image-20210201101956815.png) to get pub packagemanager.
2. If needs reopen application to reclaim package files.
   Package file reference files will be downloaded by pub package manager.
   Editing .flutter-plugins, and so on is not permitted manually. So let package manager do this.



## Android Emulator Camera Settings

For default Android Virtual Device(AVD) provides moving custom image as camera input.
So how can i change that with notebook's camera?

### Using Webcam

1. Open Android Studio
2. Open AVD Manager
3. Edit Device that using.
4. press Advance settings
5. go to Camera and change emulated image to webcam

### Using Android Emulator

Failed to find Custom Scene Image insert and picturing.



## Android Updates.

If Android Studio should be updated itself than Help Icon will show it's update news.

And if you wanna update AVD, Android Emulator and so on. follow these steps.

1. Open SDK Manager
2. Select Appropriate tab.
3. Select tools, SDKs you wanna update.





## Refactoring. Failed.

### How this app maden.

### It seems....

All thing for main screen is QrScan Class which is StatefulWidget.



### Dart grammer





## Following Flutter Tutorial

### how to add packages

1. open pubspec.yaml
2. add package you want `package: ^version` 
3. press get package button.
4. go back to source and write `import 'package:package_name';`



### Stateful widgets.

statsless widgets are immutable. so we can't change.

#### Needs

* State class
  * persists lifetime of the widget.
* StatefulWidget class
  * makes instance of State class
  * immutable
  * can be thrown away

**stful for codesnippet**



### ListView's builder factory constructor

which allows me to build a list view **lazily**



## main()'s method must be wrapped by runApp();

![image-20210201173948744](D:\KULS\DailyMD\2102\referenceImage\210221\image-20210201173948744.png)





## todo

https://flutter.dev/docs/get-started/learn-more

## currently doing

https://flutter.dev/docs/development/ui/widgets-intro