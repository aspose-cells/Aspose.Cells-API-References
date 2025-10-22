##MsoLineFormat
Represents line and arrowhead formatting.
## MsoLineFormat class
Represents line and arrowhead formatting.
```javascript
class MsoLineFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isVisible](#isVisible--)| boolean | Indicates whether the object is visible. |
| [style](#style--)| MsoLineStyle | Returns a Style object that represents the style of the specified range. |
| [foreColor](#foreColor--)| Color | Gets and sets the border line fore color. |
| [backColor](#backColor--)| Color | Gets and sets the border line back color. |
| [dashStyle](#dashStyle--)| MsoLineDashStyle | Gets or sets the dash style for the specified line. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [weight](#weight--)| number | Returns or sets the weight of the line ,in units of pt. |
## Methods
| Method | Description |
| --- | --- |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether the object is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether the object is visible. |
| [getStyle()](#getStyle--)| <b>@deprecated.</b> Please use the 'style' property instead. Returns a Style object that represents the style of the specified range. |
| [setStyle(MsoLineStyle)](#setStyle-msolinestyle-)| <b>@deprecated.</b> Please use the 'style' property instead. Returns a Style object that represents the style of the specified range. |
| [getForeColor()](#getForeColor--)| <b>@deprecated.</b> Please use the 'foreColor' property instead. Gets and sets the border line fore color. |
| [setForeColor(Color)](#setForeColor-color-)| <b>@deprecated.</b> Please use the 'foreColor' property instead. Gets and sets the border line fore color. |
| [getBackColor()](#getBackColor--)| <b>@deprecated.</b> Please use the 'backColor' property instead. Gets and sets the border line back color. |
| [setBackColor(Color)](#setBackColor-color-)| <b>@deprecated.</b> Please use the 'backColor' property instead. Gets and sets the border line back color. |
| [getDashStyle()](#getDashStyle--)| <b>@deprecated.</b> Please use the 'dashStyle' property instead. Gets or sets the dash style for the specified line. |
| [setDashStyle(MsoLineDashStyle)](#setDashStyle-msolinedashstyle-)| <b>@deprecated.</b> Please use the 'dashStyle' property instead. Gets or sets the dash style for the specified line. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [getWeight()](#getWeight--)| <b>@deprecated.</b> Please use the 'weight' property instead. Returns or sets the weight of the line ,in units of pt. |
| [setWeight(number)](#setWeight-number-)| <b>@deprecated.</b> Please use the 'weight' property instead. Returns or sets the weight of the line ,in units of pt. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### isVisible {#isVisible--}
Indicates whether the object is visible.
```javascript
isVisible : boolean;
```
### style {#style--}
Returns a Style object that represents the style of the specified range.
```javascript
style : MsoLineStyle;
```
### foreColor {#foreColor--}
Gets and sets the border line fore color.
```javascript
foreColor : Color;
```
### backColor {#backColor--}
Gets and sets the border line back color.
```javascript
backColor : Color;
```
### dashStyle {#dashStyle--}
Gets or sets the dash style for the specified line.
```javascript
dashStyle : MsoLineDashStyle;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### weight {#weight--}
Returns or sets the weight of the line ,in units of pt.
```javascript
weight : number;
```
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getStyle() {#getStyle--}
```javascript
getStyle() : MsoLineStyle;
```
**Returns**
[MsoLineStyle](../msolinestyle/)
### setStyle(MsoLineStyle) {#setStyle-msolinestyle-}
```javascript
setStyle(value: MsoLineStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |
### getForeColor() {#getForeColor--}
```javascript
getForeColor() : Color;
```
**Returns**
[Color](../color/)
### setForeColor(Color) {#setForeColor-color-}
```javascript
setForeColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getBackColor() {#getBackColor--}
```javascript
getBackColor() : Color;
```
**Returns**
[Color](../color/)
### setBackColor(Color) {#setBackColor-color-}
```javascript
setBackColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getDashStyle() {#getDashStyle--}
```javascript
getDashStyle() : MsoLineDashStyle;
```
**Returns**
[MsoLineDashStyle](../msolinedashstyle/)
### setDashStyle(MsoLineDashStyle) {#setDashStyle-msolinedashstyle-}
```javascript
setDashStyle(value: MsoLineDashStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |
### getTransparency() {#getTransparency--}
```javascript
getTransparency() : number;
```
### setTransparency(number) {#setTransparency-number-}
```javascript
setTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWeight() {#getWeight--}
```javascript
getWeight() : number;
```
### setWeight(number) {#setWeight-number-}
```javascript
setWeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
