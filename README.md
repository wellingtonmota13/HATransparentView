HATransparentView
=================

Custom `UIView` subclass based on Rdio stations menu.

![Demo HATransparentView](https://raw.github.com/hebertialmeida/HATransparentView/master/HATransparentViewDemo/Images.xcassets/1.png)
![Demo2 HATransparentView](https://raw.github.com/hebertialmeida/HATransparentView/master/HATransparentViewDemo/Images.xcassets/2.png)

Install
-----

### Installation with CocoaPods
[CocoaPods](http://cocoapods.org) is the best way to manage library dependencies in Objective-C projects.

#### Podfile
```ruby
platform :ios
pod 'HATransparentView', '~> 0.2'
```

Usage
-----
 1. Add Key value to info.plist: `View controller-based status bar appearance`, `NO`

 1. Import the header file wherever you want to use the HATransparentView:
```objc
#import "HATransparentView.h"
```

 1. Define:
```objc
@property (strong, nonatomic) HATransparentView *transparentView;
```

 1. Default open:
```objc
_transparentView = [[HATransparentView alloc] init];
[_transparentView open];
```

 1. Close:
```objc
[_transparentView close];
```

Custom
-----

 1. Custom background:
```objc
_transparentView = [[HATransparentView alloc] init];
_transparentView.backgroundColor = [UIColor colorWithRed:242/255.0 green:46/255.0 blue:50/255.0 alpha:0.9];
[_transparentView open];
```

 1. Custom status bar (iOS 7) and close button with `HAStyleBlack`, default is `HAStyleLight`:
```objc
_transparentView = [[HATransparentView alloc] init];
_transparentView.style = HAStyleBlack;
[_transparentView open];
```


Requirements
----------
* iOS 6.0 or higher
* ARC

## License
HATransparentView is released under the MIT license. See
[LICENSE](https://github.com/hebertialmeida/HATransparentView/blob/master/LICENSE).

Contact me
----------

**Heberti Almeida**  


* Contact: [hebertialmeida@gmail.com][1]
* Twitter: [http://twitter.com/hebertialmeida][2] 
* LinkedIn: [http://www.linkedin.com/in/hebertialmeida][3] 

  [1]: mailto:hebertialmeida@gmail.com
  [2]: http://twitter.com/hebertialmeida
  [3]: http://www.linkedin.com/in/hebertialmeida 


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/hebertialmeida/hatransparentview/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

