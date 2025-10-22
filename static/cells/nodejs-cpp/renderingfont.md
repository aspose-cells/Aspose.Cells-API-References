##RenderingFont
Font for rendering.
## RenderingFont class
Font for rendering.
```javascript
class RenderingFont;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(string, number)](#constructor-string-number-)| Initializes a new instance of the [RenderingFont](../renderingfont/) |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Gets name of the font. |
| [size](#size--)| number | Readonly. Gets size of the font in points. |
| [bold](#bold--)| boolean | Gets or sets bold for the font. |
| [italic](#italic--)| boolean | Gets or sets italic for the font. |
| [color](#color--)| Color | Gets or sets color for the font. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets name of the font. |
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Gets size of the font in points. |
| [getBold()](#getBold--)| <b>@deprecated.</b> Please use the 'bold' property instead. Gets or sets bold for the font. |
| [setBold(boolean)](#setBold-boolean-)| <b>@deprecated.</b> Please use the 'bold' property instead. Gets or sets bold for the font. |
| [getItalic()](#getItalic--)| <b>@deprecated.</b> Please use the 'italic' property instead. Gets or sets italic for the font. |
| [setItalic(boolean)](#setItalic-boolean-)| <b>@deprecated.</b> Please use the 'italic' property instead. Gets or sets italic for the font. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets color for the font. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets color for the font. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(string, number) {#constructor-string-number-}
Initializes a new instance of the [RenderingFont](../renderingfont/)
```javascript
constructor(fontName: string, fontSize: number);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | string | font name |
| fontSize | number | font size in points |
### name {#name--}
Readonly. Gets name of the font.
```javascript
name : string;
```
### size {#size--}
Readonly. Gets size of the font in points.
```javascript
size : number;
```
### bold {#bold--}
Gets or sets bold for the font.
```javascript
bold : boolean;
```
### italic {#italic--}
Gets or sets italic for the font.
```javascript
italic : boolean;
```
### color {#color--}
Gets or sets color for the font.
```javascript
color : Color;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### getSize() {#getSize--}
```javascript
getSize() : number;
```
### getBold() {#getBold--}
```javascript
getBold() : boolean;
```
### setBold(boolean) {#setBold-boolean-}
```javascript
setBold(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getItalic() {#getItalic--}
```javascript
getItalic() : boolean;
```
### setItalic(boolean) {#setItalic-boolean-}
```javascript
setItalic(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
