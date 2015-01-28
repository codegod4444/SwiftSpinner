# SwiftSpinner

[![Version](https://img.shields.io/cocoapods/v/SwiftSpinner.svg?style=flat)](http://cocoadocs.org/docsets/SwiftSpinner)
[![License](https://img.shields.io/cocoapods/l/SwiftSpinner.svg?style=flat)](http://cocoadocs.org/docsets/SwiftSpinner)
[![Platform](https://img.shields.io/cocoapods/p/SwiftSpinner.svg?style=flat)](http://cocoadocs.org/docsets/SwiftSpinner)

SwiftSpinner is an extra beautiful activity indicator with plain and bold style fitting iOS 8 design very well. It uses dynamic blur and translucency to overlay the current screen contents and display an activity indicator with text (or the so called “spinner”).

I developed it for my Swift app called **Doodle Doodle** and wanted to share it with everyone. Check the app here: http://doodledoodle.io

This is how the activity looks like (from the demo app):

![SwiftSpinner Screenshot](https://raw.githubusercontent.com/icanzilb/SwiftSpinner/master/etc/spinner-preview.gif)

## Usage

To run the example project, clone the repo, and run `pod install` from the Example directory first. That’ll run the demo program which shows you how the spinner looks like and what it can do. 

The simple code to get SwiftSpinner running in your own app.

1. In case you installed SwiftSpinner via CocoaPods you need to import it (add this somewhere at the top of your source code file):

    import SwiftSpinner

2. When you want to show an animated activity (eg. rings are randomly rotating around):

     SwiftSpinner.show("Connecting to satellite...")
    
3. If you want to show a static activity indicator (eg. a message with two complete rings around it)

    SwiftSpinner.show("Failed to connect, waiting...", animated: false)
    
4. When you want to hide the activity:

    SwiftSpinner.hide()

That's all. If you want to change the text of the current activity, just call `show(...)` again, this will animate the old text into the new text.
    
## Requirements

There aren’t any requirements per se. As long as you got `UIKit` imported the spinner takes care of everything else.

## Installation

SwiftSpinner is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

    pod "SwiftSpinner"

*NB*: Currently Swift Cocoapods work only with 0.36 pre-release version. If you want to learn how to install a Swift cocoapod read more here: http://blog.cocoapods.org/Pod-Authors-Guide-to-CocoaPods-Frameworks/

## Author

Marin Todorov, http://www.touch-code-magazine.com/about

## License

SwiftSpinner is available under the MIT license. See the LICENSE file for more info.

