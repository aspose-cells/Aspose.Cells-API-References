##GradientFill
Represents the gradient fill.
## GradientFill class
Represents the gradient fill.
```javascript
class GradientFill;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [gradientStops](#gradientStops--)| GradientStopCollection | Readonly. Represents the gradient stop collection. |
| [fillType](#fillType--)| GradientFillType | Readonly. Gets the gradient fill type. |
| [directionType](#directionType--)| GradientDirectionType | Readonly. Gets the gradient direction type. |
| [angle](#angle--)| number | The angle of linear fill. |
## Methods
| Method | Description |
| --- | --- |
| [setGradient(GradientFillType, number, GradientDirectionType)](#setGradient-gradientfilltype-number-gradientdirectiontype-)| Set the gradient fill type and direction. |
| [setPresetThemeGradient(PresetThemeGradientType, ThemeColorType)](#setPresetThemeGradient-presetthemegradienttype-themecolortype-)| Sets preset theme gradient fill. |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, number, Color, number, GradientStyleType, number)](#setTwoColorGradient-color-number-color-number-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
### gradientStops {#gradientStops--}
Readonly. Represents the gradient stop collection.
```javascript
gradientStops : GradientStopCollection;
```
### fillType {#fillType--}
Readonly. Gets the gradient fill type.
```javascript
fillType : GradientFillType;
```
### directionType {#directionType--}
Readonly. Gets the gradient direction type.
```javascript
directionType : GradientDirectionType;
```
### angle {#angle--}
The angle of linear fill.
```javascript
angle : number;
```
### setGradient(GradientFillType, number, GradientDirectionType) {#setGradient-gradientfilltype-number-gradientdirectiontype-}
Set the gradient fill type and direction.
```javascript
setGradient(type: GradientFillType, angle: number, direction: GradientDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [GradientFillType](../gradientfilltype/) | Gradient fill type. |
| angle | number | The angle. Only applies for GradientFillType.Linear. |
| direction | [GradientDirectionType](../gradientdirectiontype/) | The direction type. Only applies for GradientFillType.Radial and GradientFillType.Rectangle. |
### setPresetThemeGradient(PresetThemeGradientType, ThemeColorType) {#setPresetThemeGradient-presetthemegradienttype-themecolortype-}
Sets preset theme gradient fill.
```javascript
setPresetThemeGradient(gradientType: PresetThemeGradientType, themeColorType: ThemeColorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | [PresetThemeGradientType](../presetthemegradienttype/) | The preset gradient type. |
| themeColorType | [ThemeColorType](../themecolortype/) | The theme color type. |
### setOneColorGradient(Color, number, GradientStyleType, number) {#setOneColorGradient-color-number-gradientstyletype-number-}
Sets the specified fill to a one-color gradient. Only applies for Excel 2007.
```javascript
setOneColorGradient(color: Color, degree: number, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../color/) | One gradient color. |
| degree | number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setTwoColorGradient(Color, Color, GradientStyleType, number) {#setTwoColorGradient-color-color-gradientstyletype-number-}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```javascript
setTwoColorGradient(color1: Color, color2: Color, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) | One gradient color. |
| color2 | [Color](../color/) | Two gradient color. |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setTwoColorGradient(Color, number, Color, number, GradientStyleType, number) {#setTwoColorGradient-color-number-color-number-gradientstyletype-number-}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```javascript
setTwoColorGradient(color1: Color, transparency1: number, color2: Color, transparency2: number, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) | One gradient color. |
| transparency1 | number | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | [Color](../color/) | Two gradient color. |
| transparency2 | number | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
