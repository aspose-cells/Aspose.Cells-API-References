##Font
Encapsulates the font object used in a spreadsheet.
## Font class
Encapsulates the font object used in a spreadsheet.
```javascript
class Font;
```
### Example
```javascript
const { Workbook, Color, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Accessing the "A1" cell from the worksheet
var cell = worksheet.cells.get("A1");
//Adding some value to the "A1" cell
cell.putValue("Hello Aspose!");
var style = cell.getStyle();
var font = style.font;
//Setting the font name to "Times New Roman"
font.setName("Times New Roman");
//Setting font size to 14
font.setSize(14);
//setting font color as Red
font.color = Color.Red;
cell.setStyle(style);
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [charset](#charset--)| number | Represent the character set. |
| [isItalic](#isItalic--)| boolean | Gets or sets a value indicating whether the font is italic. |
| [isBold](#isBold--)| boolean | Gets or sets a value indicating whether the font is bold. |
| [capsType](#capsType--)| TextCapsType | Gets and sets the text caps type. |
| [strikeType](#strikeType--)| TextStrikeType | Gets the strike type of the text. |
| [isStrikeout](#isStrikeout--)| boolean | Gets or sets a value indicating whether the font is single strikeout. |
| [scriptOffset](#scriptOffset--)| number | Gets and sets the script offset,in unit of percentage |
| [isSuperscript](#isSuperscript--)| boolean | Gets or sets a value indicating whether the font is super script. |
| [isSubscript](#isSubscript--)| boolean | Gets or sets a value indicating whether the font is subscript. |
| [underline](#underline--)| FontUnderlineType | Gets or sets the font underline type. |
| [doubleSize](#doubleSize--)| number | Gets and sets the double size of the font. |
| [size](#size--)| number | Gets or sets the size of the font. |
| [themeColor](#themeColor--)| ThemeColor | Gets and sets the theme color. |
| [color](#color--)| Color | Gets or sets the [Color](../color/) of the font. |
| [argbColor](#argbColor--)| number | Gets and sets the color with a 32-bit ARGB value. |
| [isNormalizeHeights](#isNormalizeHeights--)| boolean | Indicates whether the normalization of height that is to be applied to the text run. |
| [schemeType](#schemeType--)| FontSchemeType | Gets and sets the scheme type of the font. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Font)](#equals-font-)| Checks if two fonts are equals. |
| [getName()](#getName--)| Gets  or sets the name of the [Font](../font/). |
| [setName(string)](#setName-string-)| Gets  or sets the name of the [Font](../font/). |
| [toString()](#toString--)| Returns a string represents the current Cell object. |
### charset {#charset--}
Represent the character set.
```javascript
charset : number;
```
### isItalic {#isItalic--}
Gets or sets a value indicating whether the font is italic.
```javascript
isItalic : boolean;
```
### isBold {#isBold--}
Gets or sets a value indicating whether the font is bold.
```javascript
isBold : boolean;
```
### capsType {#capsType--}
Gets and sets the text caps type.
```javascript
capsType : TextCapsType;
```
### strikeType {#strikeType--}
Gets the strike type of the text.
```javascript
strikeType : TextStrikeType;
```
### isStrikeout {#isStrikeout--}
Gets or sets a value indicating whether the font is single strikeout.
```javascript
isStrikeout : boolean;
```
### scriptOffset {#scriptOffset--}
Gets and sets the script offset,in unit of percentage
```javascript
scriptOffset : number;
```
### isSuperscript {#isSuperscript--}
Gets or sets a value indicating whether the font is super script.
```javascript
isSuperscript : boolean;
```
### isSubscript {#isSubscript--}
Gets or sets a value indicating whether the font is subscript.
```javascript
isSubscript : boolean;
```
### underline {#underline--}
Gets or sets the font underline type.
```javascript
underline : FontUnderlineType;
```
### doubleSize {#doubleSize--}
Gets and sets the double size of the font.
```javascript
doubleSize : number;
```
### size {#size--}
Gets or sets the size of the font.
```javascript
size : number;
```
### themeColor {#themeColor--}
Gets and sets the theme color.
```javascript
themeColor : ThemeColor;
```
**Remarks**
If the font color is not a theme color, NULL will be returned.
### color {#color--}
Gets or sets the [Color](../color/) of the font.
```javascript
color : Color;
```
### argbColor {#argbColor--}
Gets and sets the color with a 32-bit ARGB value.
```javascript
argbColor : number;
```
### isNormalizeHeights {#isNormalizeHeights--}
Indicates whether the normalization of height that is to be applied to the text run.
```javascript
isNormalizeHeights : boolean;
```
### schemeType {#schemeType--}
Gets and sets the scheme type of the font.
```javascript
schemeType : FontSchemeType;
```
### equals(Font) {#equals-font-}
Checks if two fonts are equals.
```javascript
equals(font: Font) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| font | [Font](../font/) | Compared font object. |
**Returns**
True if equal to the compared font object.
### getName() {#getName--}
Gets  or sets the name of the [Font](../font/).
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
Gets  or sets the name of the [Font](../font/).
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Example**
```javascript
const { Workbook } = AsposeCells;
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Accessing the "A1" cell from the worksheet
var cell = worksheet.cells.get("A1");
//Adding some value to the "A1" cell
cell.putValue("Hello Aspose!");
var style = cell.getStyle();
var font = style.font;
font.setName("Times New Roman");
cell.setStyle(style);
```
### toString() {#toString--}
Returns a string represents the current Cell object.
```javascript
toString() : string;
```
