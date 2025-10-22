##Floor
Encapsulates the object that represents the floor of a 3D chart.
## Floor class
Encapsulates the object that represents the floor of a 3-D chart.
```javascript
class Floor extends Area;
```
### Example
```javascript
const { License, Workbook, ChartType, Color, GradientPresetType, GradientStyleType } = require("aspose.cells.node");
//Instantiate the License class
var license = new License();
license.setLicense("input/Aspose.Cells.lic");
//Instantiate the workbook object
var workbook = new Workbook();
//Get cells collection
var cells = workbook.worksheets.get(0).cells;
//Put values in cells
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
cells.get("A3").putValue(3);
//get charts colletion
var charts = workbook.worksheets.get(0).charts;
//add a new chart
var index = charts.add(ChartType.Column3DStacked, 5, 0, 15, 5);
//get the newly added chart
var chart = charts.get(index);
//set charts nseries
chart.nSeries.add("A1:A3", true);
//Show data labels
chart.nSeries.get(0).dataLabels.showValue = true;
//Get chart's floor
var floor = chart.floor;
//set floor's border as red
floor.border.color = new Color("red");
//set fill format
floor.fillFormat.setPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);
//save the file
workbook.save("output/ChartsFloor.xls");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Area)](#constructor-area-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [border](#border--)| Line | Gets or sets the border [Line](../line/). |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Gets or sets the border [Line](../line/). |
| [setBorder(Line)](#setBorder-line-)| <b>@deprecated.</b> Please use the 'border' property instead. Gets or sets the border [Line](../line/). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### constructor(Area) {#constructor-area-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Area);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Area | The parent object. |
### border {#border--}
Gets or sets the border [Line](../line/).
```javascript
border : Line;
```
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
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### setBorder(Line) {#setBorder-line-}
```javascript
setBorder(value: Line) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Line](../line/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
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
