##Column
Represents a single column in a worksheet.
## Column class
Represents a single column in a worksheet.
```javascript
class Column;
```
### Example
```javascript
const { Workbook, Color, BackgroundType, StyleFlag, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the first worksheet
var worksheet = workbook.worksheets.get(0);
//Add new Style to Workbook
var style = workbook.createStyle();
//Setting the background color to Blue
style.backgroundColor = Color.Blue;
//Setting the foreground color to Red
style.foregroundColor = Color.Red;
//setting Background Pattern
style.pattern = BackgroundType.DiagonalStripe;
//New Style Flag
var styleFlag = new StyleFlag();
//Set All Styles
styleFlag.all = true;
//Get first Column
var column = worksheet.cells.columns.get(0);
//Apply Style to first Column
column.applyStyle(style, styleFlag);
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [index](#index--)| number | Readonly. Gets the index of this column. |
| [width](#width--)| number | Gets and sets the column width in unit of characters. |
| [groupLevel](#groupLevel--)| number | Gets the group level of the column. |
| [isHidden](#isHidden--)| boolean | Indicates whether the column is hidden. |
| [hasCustomStyle](#hasCustomStyle--)| boolean | Readonly. Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [isCollapsed](#isCollapsed--)| boolean | whether the column is collapsed |
## Methods
| Method | Description |
| --- | --- |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole column. |
| [getStyle()](#getStyle--)| Gets the style of this column. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of this column. |
### index {#index--}
Readonly. Gets the index of this column.
```javascript
index : number;
```
### width {#width--}
Gets and sets the column width in unit of characters.
```javascript
width : number;
```
**Remarks**
For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### groupLevel {#groupLevel--}
Gets the group level of the column.
```javascript
groupLevel : number;
```
### isHidden {#isHidden--}
Indicates whether the column is hidden.
```javascript
isHidden : boolean;
```
### hasCustomStyle {#hasCustomStyle--}
Readonly. Indicates whether this column has custom style settings(different from the default one inherited from workbook).
```javascript
hasCustomStyle : boolean;
```
### isCollapsed {#isCollapsed--}
whether the column is collapsed
```javascript
isCollapsed : boolean;
```
### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}
Applies formats for a whole column.
```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |
### getStyle() {#getStyle--}
Gets the style of this column.
```javascript
getStyle() : Style;
```
**Returns**
[Style](../style/)
**Remarks**
Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/) or [SetStyle(Style)](../setstyle(style)/) method to apply the change to this column.<br></br> Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### setStyle(Style) {#setStyle-style-}
Sets the style of this column.
```javascript
setStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | the style to be used as the default style for cells in this column. |
**Remarks**
This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/)
