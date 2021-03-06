<!--docs:
title: "Color Theming"
layout: detail
section: components
excerpt: "How to theme Tabs using the Material Design color system."
iconId: tabs
path: /catalog/tabs/color-theming/
-->

# Tabs Color Theming

You can theme a tab bar with your app's color scheme using the ColorThemer extension.

You must first add the Color Themer extension to your project:

``` bash
pod 'MaterialComponents/Tabs+Extensions/ColorThemer'
```

## Example code

<!--<div class="material-code-render" markdown="1">-->
#### Swift
``` swift
// Step 1: Import the ColorThemer extension
import MaterialComponents.MaterialTabs_ColorThemer

// Step 2: Create or get a color scheme
let colorScheme = MDCSemanticColorScheme()

// Step 3: Apply the color scheme to your component
// Primary variant
MDCTabBarColorThemer.applySemanticColorScheme(colorScheme, toTabs: component)
// Or surface variant
MDCTabBarColorThemer.applySurfaceVariant(withColorScheme: colorScheme, toTabs: component)
```

#### Objective-C

``` objc
// Step 1: Import the ColorThemer extension
#import "MaterialTabs+ColorThemer.h"

// Step 2: Create or get a color scheme
id<MDCColorScheming> colorScheme = [[MDCSemanticColorScheme alloc] init];

// Step 3: Apply the color scheme to your component
// Primary variant
[MDCTabBarColorThemer applySemanticColorScheme:colorScheme toTabs:component];
// Or surface variant
[MDCTabBarColorThemer applySurfaceVariantWithColorScheme:colorScheme toTabs:component];
```
<!--</div>-->
