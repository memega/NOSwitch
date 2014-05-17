## NOSwitch

A subclass of NSButton which looks similar to the UISwitch control in iOS7

![alt text](http://i.imgur.com/18RooVw.jpg "NOSwitch demo")

### Usage

Place a `Check Box` in your **nib** and select it. Open Utilities→Identity Inspector (`⌥⌘3`) and assign `NOSwitchButton` class.

Or create it in code:

```obj-c
#import "NOSwitchButton.h"

NOSwitchButton *button = [[NOSwitchButton alloc] initWithFrame:NSMakeRect(0,0,60,36)];
[self.window.contentView addSubview:button];
```

### Customization

By default, `NOSwitchButton` uses the same <span style="background-color:#55DD75;padding:1px 4px;border-radius:3px;">shade of green</span> as UISwitch in iOS7. You can change it with `tintColor` property:

```obj-c
button.tintColor = [NSColor colorWithCalibratedHue:0.05 saturation:0.86 brightness:0.99 alpha:1];
```

### Limitations

* Does not support `NSMixedState`. An attempt to set `allowsMixedState` to `YES` will have no effect.

* This control does not display neither text value nor custom image.

### License

This project is licensed under the terms of the [MIT license](http://memega.mit-license.org/).
