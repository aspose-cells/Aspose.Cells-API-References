---
title: GradientFill
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the gradient fill.
type: docs
url: /nodejs-cpp/gradientfill/
---

## GradientFill class

Represents the gradient fill.

```javascript
class GradientFill;
```


## Methods

| Method | Description |
| --- | --- |
| [getGradientStops()](#getGradientStops--)| Represents the gradient stop collection. |
| [getFillType()](#getFillType--)| Gets the gradient fill type. |
| [getDirectionType()](#getDirectionType--)| Gets the gradient direction type. |
| [getAngle()](#getAngle--)| The angle of linear fill. |
| [setAngle(number)](#setAngle-number-)| The angle of linear fill. |
| [setGradient(GradientFillType, number, GradientDirectionType)](#setGradient-gradientfilltype-number-gradientdirectiontype-)| Set the gradient fill type and direction. |
| [setPresetThemeGradient(PresetThemeGradientType, ThemeColorType)](#setPresetThemeGradient-presetthemegradienttype-themecolortype-)| Sets preset theme gradient fill. |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, number, Color, number, GradientStyleType, number)](#setTwoColorGradient-color-number-color-number-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |


### getGradientStops() {#getGradientStops--}

Represents the gradient stop collection.

```javascript
getGradientStops() : GradientStopCollection;
```


**Returns**

[GradientStopCollection](/nodejs-cpp/gradientstopcollection/)

### getFillType() {#getFillType--}

Gets the gradient fill type.

```javascript
getFillType() : GradientFillType;
```


**Returns**

[GradientFillType](/nodejs-cpp/gradientfilltype/)

### getDirectionType() {#getDirectionType--}

Gets the gradient direction type.

```javascript
getDirectionType() : GradientDirectionType;
```


**Returns**

[GradientDirectionType](/nodejs-cpp/gradientdirectiontype/)

### getAngle() {#getAngle--}

The angle of linear fill.

```javascript
getAngle() : number;
```


### setAngle(number) {#setAngle-number-}

The angle of linear fill.

```javascript
setAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### setGradient(GradientFillType, number, GradientDirectionType) {#setGradient-gradientfilltype-number-gradientdirectiontype-}

Set the gradient fill type and direction.

```javascript
setGradient(type: GradientFillType, angle: number, direction: GradientDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [GradientFillType](/nodejs-cpp/gradientfilltype/) | Gradient fill type. |
| angle | number | The angle. Only applies for GradientFillType.Linear. |
| direction | [GradientDirectionType](/nodejs-cpp/gradientdirectiontype/) | The direction type. Only applies for GradientFillType.Radial and GradientFillType.Rectangle. |

### setPresetThemeGradient(PresetThemeGradientType, ThemeColorType) {#setPresetThemeGradient-presetthemegradienttype-themecolortype-}

Sets preset theme gradient fill.

```javascript
setPresetThemeGradient(gradientType: PresetThemeGradientType, themeColorType: ThemeColorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | [PresetThemeGradientType](/nodejs-cpp/presetthemegradienttype/) | The preset gradient type. |
| themeColorType | [ThemeColorType](/nodejs-cpp/themecolortype/) | The theme color type. |

### setOneColorGradient(Color, number, GradientStyleType, number) {#setOneColorGradient-color-number-gradientstyletype-number-}

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

```javascript
setOneColorGradient(color: Color, degree: number, style: GradientStyleType, variant: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](/nodejs-cpp/color/) | One gradient color. |
| degree | number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | [GradientStyleType](/nodejs-cpp/gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(Color, Color, GradientStyleType, number) {#setTwoColorGradient-color-color-gradientstyletype-number-}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

```javascript
setTwoColorGradient(color1: Color, color2: Color, style: GradientStyleType, variant: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](/nodejs-cpp/color/) | One gradient color. |
| color2 | [Color](/nodejs-cpp/color/) | Two gradient color. |
| style | [GradientStyleType](/nodejs-cpp/gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(Color, number, Color, number, GradientStyleType, number) {#setTwoColorGradient-color-number-color-number-gradientstyletype-number-}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

```javascript
setTwoColorGradient(color1: Color, transparency1: number, color2: Color, transparency2: number, style: GradientStyleType, variant: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](/nodejs-cpp/color/) | One gradient color. |
| transparency1 | number | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | [Color](/nodejs-cpp/color/) | Two gradient color. |
| transparency2 | number | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | [GradientStyleType](/nodejs-cpp/gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |


