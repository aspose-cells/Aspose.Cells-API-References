##Area
Encapsulates the object that represents an area format.
## Area class
Encapsulates the object that represents an area format.
```javascript
class Area;
```
### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Workbook object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.nSeries.add("A1:B3", true);
//Setting the foreground color of the plot area
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Setting the foreground color of the chart area
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Setting the foreground color of the 1st NSeries area
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Setting the foreground color of the area of the 1st NSeries point
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Saving the Excel file
workbook.save("output/DrawingArea.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [getFormatting()](#getFormatting--)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| <b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### backgroundColor {#backgroundColor--}
Gets or sets the background [Color](../color/) of the [Area](../area/).
```javascript
backgroundColor : Color;
```
### foregroundColor {#foregroundColor--}
Gets or sets the foreground [Color](../color/).
```javascript
foregroundColor : Color;
```
### formatting {#formatting--}
Represents the formatting of the area.
```javascript
formatting : FormattingType;
```
### invertIfNegative {#invertIfNegative--}
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
```javascript
invertIfNegative : boolean;
```
**Example**
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Workbook object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(-100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Setting the foreground color of the 1st NSeries area
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Setting the background color of the 1st NSeries area.
//The displayed area color of second chart point will be the background color.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Saving the Excel file
workbook.save("output/DrawingAreaInverseIfNegative.xls");
```
### fillFormat {#fillFormat--}
Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.
```javascript
fillFormat : FillFormat;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### getBackgroundColor() {#getBackgroundColor--}
```javascript
getBackgroundColor() : Color;
```
**Returns**
[Color](../color/)
### setBackgroundColor(Color) {#setBackgroundColor-color-}
```javascript
setBackgroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getForegroundColor() {#getForegroundColor--}
```javascript
getForegroundColor() : Color;
```
**Returns**
[Color](../color/)
### setForegroundColor(Color) {#setForegroundColor-color-}
```javascript
setForegroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getFormatting() {#getFormatting--}
```javascript
getFormatting() : FormattingType;
```
**Returns**
[FormattingType](../formattingtype/)
### setFormatting(FormattingType) {#setFormatting-formattingtype-}
```javascript
setFormatting(value: FormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |
### getInvertIfNegative() {#getInvertIfNegative--}
```javascript
getInvertIfNegative() : boolean;
```
### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}
```javascript
setInvertIfNegative(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFillFormat() {#getFillFormat--}
```javascript
getFillFormat() : FillFormat;
```
**Returns**
[FillFormat](../fillformat/)
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
