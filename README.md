#BButton 2.0

BButton is a subclass of UIButton that looks like the [Twitter Bootstrap 2.3.1](http://twitter.github.com/bootstrap) buttons.

Refactored by [@jessesquires](http://github.com/jessesquires), April 2013.

Includes [@leberwurstsaft / FontAwesome-for-iOS](https://github.com/leberwurstsaft/FontAwesome-for-iOS), fixed for iOS from the original [FontAwesome](http://fortawesome.github.com/Font-Awesome/).

![BButton Screenshot 1][img1] &nbsp;&nbsp;&nbsp;&nbsp; ![BButton Screenshot 2][img2]

### Notable changes

* Up-to-date for iOS 5.0+, ARC, Storyboards
* Custom initialization methods for easier creation
* Option to show button 'disabled' state
* New button type options
* FontAwesome already included
* Refactored to be much cleaner, better organized

## Installation

### From [CocoaPods](http://www.cocoapods.org)

	pod 'BButton'

### From source

* Drag the `BButton/` folder to your project (make sure you copy all files/folders)
* `#import "BButton.h"`
* Add `Fonts provided by application` key to `Info.plist` and include `FontAwesome.ttf`

<img src="http://imageshack.us/a/img339/9596/bbuttonfontawesomexcode.png">

## How To Use

### With Storyboards

Create a `UIButton` and change its class to `BButton`

<img width=261 src="http://img827.imageshack.us/img827/6596/ibbbutton.png"/>

Under 'User Defined Runtime Attributes' Define At Least Type to a integer of your choice. Other properties can be set this way for additional styling.

<img width="516" height="206" src="http://i.imgur.com/NsarwUS.png"/>

### Create programmatically

Initialize with any of the following methods:

````objective-c
- (id)initWithFrame:(CGRect)frame type:(BButtonType)type
- (id)initWithFrame:(CGRect)frame type:(BButtonType)type icon:(FAIcon)icon fontSize:(CGFloat)fontSize
- (id)initWithFrame:(CGRect)frame color:(UIColor *)aColor
- (id)initWithFrame:(CGRect)frame color:(UIColor *)aColor icon:(FAIcon)icon fontSize:(CGFloat)fontSize
+ (BButton *)awesomeButtonWithOnlyIcon:(FAIcon)icon type:(BButtonType)type
+ (BButton *)awesomeButtonWithOnlyIcon:(FAIcon)icon color:(UIColor *)color
````

**See the included demo project `BButtonDemo.xcodeproj`**

**See `FontAwesomeIcons.html` for list of icons**

## Apps Using This Control

[Hemoglobe](http://bit.ly/hemoglobeapp)

[iPaint uPaint](http://bit.ly/ipupappstr)

[Audiotrip](https://itunes.apple.com/us/app/audiotrip/id569634193?mt=8&ign-mpt=uo%3D4)

*[Contact me](mailto:me@mathieubolard.com) to have your app listed here.*

##[BButton](https://github.com/mattlawer/BButton) License

[MIT License](http://opensource.org/licenses/MIT)

Copyright (c) 2013 Mathieu Bolard

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

##[FontAwesome](https://github.com/FortAwesome/Font-Awesome) License

* The Font Awesome font is licensed under the [SIL Open Font License](http://scripts.sil.org/OFL)
* Font Awesome CSS, LESS, and SASS files are licensed under the [MIT License](http://opensource.org/licenses/mit-license.html)
* The Font Awesome pictograms are licensed under the [CC BY 3.0 License](http://creativecommons.org/licenses/by/3.0)
* Attribution is no longer required in Font Awesome 3.0, but much appreciated:
	* *"Font Awesome by Dave Gandy - http://fortawesome.github.com/Font-Awesome"*

[img1]:https://raw.github.com/mattlawer/BButton/master/Screenshots/screenshot-1.png
[img2]:https://raw.github.com/mattlawer/BButton/master/Screenshots/screenshot-2.png

##Contact

mattlawer08@gmail.com<br />
http://mathieubolard.com<br />
http://twitter.com/mattlawer