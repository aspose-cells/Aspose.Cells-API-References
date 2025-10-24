##TextEffectFormat
Contains properties and methods that apply to WordArt objects.
## TextEffectFormat class
Contains properties and methods that apply to WordArt objects.
```javascript
class TextEffectFormat;
```
### Example
```javascript
const { Workbook, MsoPresetTextEffect } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
var shapes = workbook.worksheets.get(0).shapes;
shapes.addTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
var textEffectFormat = shapes.get(0).textEffect;
textEffectFormat.setTextEffect(MsoPresetTextEffect.TextEffect10);
workbook.save("output/TextEffectFormat.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [text](#text--)| string | The text in the WordArt. |
| [fontName](#fontName--)| string | The name of the font used in the WordArt. |
| [fontBold](#fontBold--)| boolean | Indicates whether font is bold. |
| [fontItalic](#fontItalic--)| boolean | Indicates whether font is italic. |
| [rotatedChars](#rotatedChars--)| boolean | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [fontSize](#fontSize--)| number | The size (in points) of the font used in the WordArt. |
| [presetShape](#presetShape--)| MsoPresetTextEffectShape | Gets and sets the preset shape type. |
## Methods
| Method | Description |
| --- | --- |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. The text in the WordArt. |
| [setText(string)](#setText-string-)| <b>@deprecated.</b> Please use the 'text' property instead. The text in the WordArt. |
| [getFontName()](#getFontName--)| <b>@deprecated.</b> Please use the 'fontName' property instead. The name of the font used in the WordArt. |
| [setFontName(string)](#setFontName-string-)| <b>@deprecated.</b> Please use the 'fontName' property instead. The name of the font used in the WordArt. |
| [getFontBold()](#getFontBold--)| <b>@deprecated.</b> Please use the 'fontBold' property instead. Indicates whether font is bold. |
| [setFontBold(boolean)](#setFontBold-boolean-)| <b>@deprecated.</b> Please use the 'fontBold' property instead. Indicates whether font is bold. |
| [getFontItalic()](#getFontItalic--)| <b>@deprecated.</b> Please use the 'fontItalic' property instead. Indicates whether font is italic. |
| [setFontItalic(boolean)](#setFontItalic-boolean-)| <b>@deprecated.</b> Please use the 'fontItalic' property instead. Indicates whether font is italic. |
| [getRotatedChars()](#getRotatedChars--)| <b>@deprecated.</b> Please use the 'rotatedChars' property instead. If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [setRotatedChars(boolean)](#setRotatedChars-boolean-)| <b>@deprecated.</b> Please use the 'rotatedChars' property instead. If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [getFontSize()](#getFontSize--)| <b>@deprecated.</b> Please use the 'fontSize' property instead. The size (in points) of the font used in the WordArt. |
| [setFontSize(number)](#setFontSize-number-)| <b>@deprecated.</b> Please use the 'fontSize' property instead. The size (in points) of the font used in the WordArt. |
| [getPresetShape()](#getPresetShape--)| <b>@deprecated.</b> Please use the 'presetShape' property instead. Gets and sets the preset shape type. |
| [setPresetShape(MsoPresetTextEffectShape)](#setPresetShape-msopresettexteffectshape-)| <b>@deprecated.</b> Please use the 'presetShape' property instead. Gets and sets the preset shape type. |
| [setTextEffect(MsoPresetTextEffect)](#setTextEffect-msopresettexteffect-)| Sets the preset text effect. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### text {#text--}
The text in the WordArt.
```javascript
text : string;
```
### fontName {#fontName--}
The name of the font used in the WordArt.
```javascript
fontName : string;
```
### fontBold {#fontBold--}
Indicates whether font is bold.
```javascript
fontBold : boolean;
```
### fontItalic {#fontItalic--}
Indicates whether font is italic.
```javascript
fontItalic : boolean;
```
### rotatedChars {#rotatedChars--}
If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape.
```javascript
rotatedChars : boolean;
```
### fontSize {#fontSize--}
The size (in points) of the font used in the WordArt.
```javascript
fontSize : number;
```
### presetShape {#presetShape--}
Gets and sets the preset shape type.
```javascript
presetShape : MsoPresetTextEffectShape;
```
### getText() {#getText--}
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFontName() {#getFontName--}
```javascript
getFontName() : string;
```
### setFontName(string) {#setFontName-string-}
```javascript
setFontName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFontBold() {#getFontBold--}
```javascript
getFontBold() : boolean;
```
### setFontBold(boolean) {#setFontBold-boolean-}
```javascript
setFontBold(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFontItalic() {#getFontItalic--}
```javascript
getFontItalic() : boolean;
```
### setFontItalic(boolean) {#setFontItalic-boolean-}
```javascript
setFontItalic(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRotatedChars() {#getRotatedChars--}
```javascript
getRotatedChars() : boolean;
```
### setRotatedChars(boolean) {#setRotatedChars-boolean-}
```javascript
setRotatedChars(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFontSize() {#getFontSize--}
```javascript
getFontSize() : number;
```
### setFontSize(number) {#setFontSize-number-}
```javascript
setFontSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPresetShape() {#getPresetShape--}
```javascript
getPresetShape() : MsoPresetTextEffectShape;
```
**Returns**
[MsoPresetTextEffectShape](../msopresettexteffectshape/)
### setPresetShape(MsoPresetTextEffectShape) {#setPresetShape-msopresettexteffectshape-}
```javascript
setPresetShape(value: MsoPresetTextEffectShape) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoPresetTextEffectShape](../msopresettexteffectshape/) | The value to set. |
### setTextEffect(MsoPresetTextEffect) {#setTextEffect-msopresettexteffect-}
Sets the preset text effect.
```javascript
setTextEffect(effect: MsoPresetTextEffect) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | [MsoPresetTextEffect](../msopresettexteffect/) | The preset text effect. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
