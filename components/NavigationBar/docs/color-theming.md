<!--docs:
title: "Color Theming"
layout: detail
section: components
excerpt: "How to theme Navigation Bar using the Material Design color system."
iconId: toolbar
path: /catalog/flexible-headers/navigation-bars/color-theming/
-->

# Navigation Bar Color Theming

You can theme a navigation bar with your app's color scheme using the ColorThemer extension.

You must first add the Color Themer extension to your project:

``` bash
pod 'MaterialComponents/NavigationBar+Extensions/ColorThemer'
```

## Example code

<!--<div class="material-code-render" markdown="1">-->
#### Swift
``` swift
// Step 1: Import the ColorThemer extension
import MaterialComponents.MaterialNavigationBar_ColorThemer

// Step 2: Create or get a color scheme
let colorScheme = MDCSemanticColorScheme()

// Step 3: Apply the color scheme to your component
MDCNavigationBarColorThemer.applySemanticColorScheme(colorScheme, to: component)
```

#### Objective-C

``` objc
// Step 1: Import the ColorThemer extension
#import "MaterialNavigationBar+ColorThemer.h"

// Step 2: Create or get a color scheme
id<MDCColorScheming> colorScheme = [[MDCSemanticColorScheme alloc] init];

// Step 3: Apply the color scheme to your component
[MDCNavigationBarColorThemer applySemanticColorScheme:colorScheme
     toNavigationBar:component];
```
<!--</div>-->
