##TextEffectFormat
Contains properties and methods that apply to WordArt objects.
## TextEffectFormat class
Contains properties and methods that apply to WordArt objects.
```javascript
class TextEffectFormat;
```
### Example
```javascript
const { Workbook, MsoPresetTextEffect, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
var shapes = workbook.worksheets.get(0).shapes;
shapes.addTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
var textEffectFormat = shapes.get(0).textEffect;
textEffectFormat.setTextEffect(MsoPresetTextEffect.TextEffect10);
var uint8Array = workbook.save(SaveFormat.Xlsx);
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
| [setTextEffect(MsoPresetTextEffect)](#setTextEffect-msopresettexteffect-)| Sets the preset text effect. |
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
### setTextEffect(MsoPresetTextEffect) {#setTextEffect-msopresettexteffect-}
Sets the preset text effect.
```javascript
setTextEffect(effect: MsoPresetTextEffect) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | [MsoPresetTextEffect](../msopresettexteffect/) | The preset text effect. |
