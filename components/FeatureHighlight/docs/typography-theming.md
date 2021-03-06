<!--docs:
title: "Typography Theming"
layout: detail
section: components
excerpt: "How to theme Feature Highlight using the Material Design typography system."
iconId: feature_highlight
path: /catalog/feature-highlights/typography-theming/
-->

# Feature Highlight Typography Theming

You can theme feature highlight with your app's typography scheme using the TypographyThemer extension.

You must first add the Typography Themer extension to your project:

``` bash
pod 'MaterialComponents/FeatureHighlight+Extensions/TypographyThemer'
```

## Example code

<!--<div class="material-code-render" markdown="1">-->
#### Swift
``` swift
// Step 1: Import the TypographyThemer extension
import MaterialComponents.MaterialFeatureHighlight_TypographyThemer

// Step 2: Create or get a typography scheme
let typographyScheme = MDCTypographyScheme()

// Step 3: Apply the typography scheme to your component
MDCFeatureHighlightTypographyThemer.applyTypographyScheme(typographyScheme, to: component)
```

#### Objective-C

``` objc
// Step 1: Import the TypographyThemer extension
#import "MaterialFeatureHighlight+TypographyThemer.h"

// Step 2: Create or get a typography scheme
id<MDCTypographyScheming> typographyScheme = [[MDCTypographyScheme alloc] init];

// Step 3: Apply the typography scheme to your component
[MDCFeatureHighlightTypographyThemer applyTypographyScheme:colorScheme
     toFeatureHighlightViewController:component];
```
<!--</div>-->
