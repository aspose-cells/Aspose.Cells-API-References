##Border
Encapsulates the object that represents the cell border.
## Border class
Encapsulates the object that represents the cell border.
```javascript
class Border;
```
### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color } = AsposeCells;
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
