### DTCoreText-DEMO
Executable Demo project in https://github.com/Cocoanetics/DTCoreText

<br>Cocoanetics, Oliver Drobnik is the original author of the DTCoreText and DTCoreDemo.
<br>The original source code can be find at https://github.com/Cocoanetics/DTCoreText.

###Why?
Yes, probablly author already have put right instructions to run Demo.
<br>Yes, this repo can be removable upon request by author.

But, I really had short time for finding an instructions and addressing build issue(s) to run Demo project.

###What is included?
Podfile pointing to original author's repositories.
Demo project from original author.

###Who to follow?
https://github.com/Cocoanetics/DTCoreText
and follow the license information.

###How to build this Demo?
```objective-c
// you must have a cocoapods 
// run this in terminal
pod install

// You will get a build error 
// add this MACRO to DTCompatibility.h in Pods->DTCoreText
#if __IPHONE_OS_VERSION_MAX_ALLOWED > 80400
#define DT_SUPPORTED_INTERFACE_ORIENTATIONS_RETURN_TYPE UIInterfaceOrientationMask
#else
#define DT_SUPPORTED_INTERFACE_ORIENTATIONS_RETURN_TYPE NSUInteger
#endif
// There are also same file `DTCompatibility.h` file in DTFoundation... that has above MACRO
// Ready to execute!
```
