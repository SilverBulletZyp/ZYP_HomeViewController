# ZYP_HomeViewController


## How to build?


* initialize Podfile

```vim
vim Podfile
```

* input

```ruby
project "xxx.xcodeproj"

platform:ios,'xxx'
inhibit_all_warnings!
target 'xxx' do
pod 'ZYP_HomeViewController', '1.0.5'
end
```

* update

```vim
pod update
```

## How to use?


* input class name in `AppDelegate.m`

```
#import "AppDelegate.h"
#import "ZYP_HomeViewController.h"
```

* function `didFinishLaunchingWithOptions` add content

```objective-c
NSArray *array = @[@{@"name":@"Title 1",@"vc":@"ClassName1"},@{@"name":@"Title 2",@"vc":@"ClassName2"},];
ZYPNavigationController *nav = [[ZYPNavigationController alloc]initWithTitle:@"HomeTitle" vcArray:array];
self.window.rootViewController = nav;
```
