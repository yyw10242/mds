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

always the starting point is 

```dart
void main() => runApp
```

don't forget.



## Basic Widgets

### Text

just some kind of text box.

### Row, Column

privides flexible layout which based web's flexbox layout model.

### Stack

like web's absolute positioning layout model.

> use Positioned Widget to set relatively to the top, right, left , bottom

### Container

let us to create a rectanglar visual element. can be decorated with  BoxDecoration Widget. Which allows us adjust background, border, shadow.

As this widget offer us **Rectangular** visual element, this can have margin, padding, and so on



## Using Material Components

### Scaffold

#### Contains

* appBar
* body
* and..so on. quite lot

Anyway it is not just only appbar. it's more lika panel which have appBar

<img src="referenceImage/Flutter/image-20210203101802694.png" alt="image-20210203101802694" style="zoom:%;" />

### AppBar

![image-20210203101831657](referenceImage/Flutter/image-20210203101831657.png)

bottom: generally used for TabBar. which is not goal of mine so move on.

### DefaultTabController

which needs **3** widgets

* DefaultTabController
* TabBar
  locates AppBar's bottom
* TabBarView
  locates DefaultTabController's body



### Stateless Widget and Stateful Widget.

#### Stateless Widget

immutable. so once setted it can't be change.

#### Stateful widget

can have mutable variables. and 



### Main, Cross Axis Alignment

`mainAxisAlignment` and `crossAxisAlignment` is the property of Column, Row Elements.

main is main direction and cross is crossed direction



## How this tutorial made spaces.

### padding in Container Widget

```dart
 padding: const EdgeInsets.only(botton: 8),
```



## Animate a widget across screens

### Hero

which privides same image transition.

Each Screen widget need to have `Hero Widget with same tag`

and then just `Navigator.push(context, MaterialPageRoute(builder:(_){return DetailScreen();}))`



## Navigate to a new screen and back

* Navigator.push
* Navigator.pop



## Pass arguments

In this Example it was confusing because two suggestion was suggested.

first is using `onGenerateRoute` event inside of MaterialApp.



Both method needs same call method.

```dart
Navigator.pushNamed(
                  context,
                  targetScreen.routeName,
                  arguments: argumentDataClass(
                    'arg1',
                    'arg2',
                  ),
                );
```



#### get Arguments with BuildContext

* using MaterialApp's routes
  * when target route comes then returns assigned widget.

```dart
/// inside of MaterialApp
routes: {
          ExtractArgumentsScreen.routeName: (context) =>
              ExtractArgumentsScreen(),
        });
```



#### get Arguments with onGenerateRoute event

* using MaterialApp's onGenerateRoute
  * When Route generates, **onGenerateRoute** event calls. 
    So this event can get route name and using that parameter 
    returns appropriate widget.
  * We can handle routes didn't made by

```dart
assert(false, 'Need to implement ${settings.name}');
```

## How can we use this...

Actually i don't know hoe to use this mehods.

but if i can..

i can make screen like this

  if session available

Splash - login page - main page

​	     - main page



## Return Data From screen

using async await.

we can get return value from other Screen

and `Navigator.pop` have a result parameter to toss result value.

so..

>  Navigator.pop<T>(context, <T>value)

to return value.

### Scaffold's SnackBar Widget(?)

Scaffold have a snackBar. Which is 



## Drawer

> Is a sideBar.

Think like... Yugioh's `draw!`

then side bar slides to screen

else... just press hamburger button.



## todo

https://flutter.dev/docs/get-started/learn-more

