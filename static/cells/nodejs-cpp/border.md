##Border
Encapsulates the object that represents the cell border.
## Border class
Encapsulates the object that represents the cell border.
```javascript
class Border;
```
### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color } = require("aspose.cells.node");
var workbook = new Workbook();
var worksheet = workbook.worksheets.get(0);
var cell = worksheet.cells.get(0, 0);
var style = workbook.createStyle();
//Set top border style and color
var border = style.borders.get(BorderType.TopBorder);
border.lineStyle = CellBorderType.Medium;
border.color = Color.Red;
cell.setStyle(style);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [themeColor](#themeColor--)| ThemeColor | Gets and sets the theme color of the border. |
| [color](#color--)| Color | Gets or sets the [Color](../color/) of the border. |
| [argbColor](#argbColor--)| number | Gets and sets the color with a 32-bit ARGB value. |
| [lineStyle](#lineStyle--)| CellBorderType | Gets or sets the cell border type. |
## Methods
| Method | Description |
| --- | --- |
| [getThemeColor()](#getThemeColor--)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color of the border. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color of the border. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/) of the border. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/) of the border. |
| [getArgbColor()](#getArgbColor--)| <b>@deprecated.</b> Please use the 'argbColor' property instead. Gets and sets the color with a 32-bit ARGB value. |
| [setArgbColor(number)](#setArgbColor-number-)| <b>@deprecated.</b> Please use the 'argbColor' property instead. Gets and sets the color with a 32-bit ARGB value. |
| [getLineStyle()](#getLineStyle--)| <b>@deprecated.</b> Please use the 'lineStyle' property instead. Gets or sets the cell border type. |
| [setLineStyle(CellBorderType)](#setLineStyle-cellbordertype-)| <b>@deprecated.</b> Please use the 'lineStyle' property instead. Gets or sets the cell border type. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### themeColor {#themeColor--}
Gets and sets the theme color of the border.
```javascript
themeColor : ThemeColor;
```
### color {#color--}
Gets or sets the [Color](../color/) of the border.
```javascript
color : Color;
```
### argbColor {#argbColor--}
Gets and sets the color with a 32-bit ARGB value.
```javascript
argbColor : number;
```
### lineStyle {#lineStyle--}
Gets or sets the cell border type.
```javascript
lineStyle : CellBorderType;
```
### getThemeColor() {#getThemeColor--}
```javascript
getThemeColor() : ThemeColor;
```
**Returns**
[ThemeColor](../themecolor/)
### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}
```javascript
setThemeColor(value: ThemeColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |
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
### getArgbColor() {#getArgbColor--}
```javascript
getArgbColor() : number;
```
### setArgbColor(number) {#setArgbColor-number-}
```javascript
setArgbColor(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLineStyle() {#getLineStyle--}
```javascript
getLineStyle() : CellBorderType;
```
**Returns**
[CellBorderType](../cellbordertype/)
### setLineStyle(CellBorderType) {#setLineStyle-cellbordertype-}
```javascript
setLineStyle(value: CellBorderType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellBorderType](../cellbordertype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
