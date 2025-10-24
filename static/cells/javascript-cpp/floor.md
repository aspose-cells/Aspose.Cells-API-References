##Floor
Encapsulates the object that represents the floor of a 3D chart.
## Floor class
Encapsulates the object that represents the floor of a 3-D chart.
```javascript
class Floor extends Area;
```
### Example
```javascript
const { License, Workbook, ChartType, Color, GradientPresetType, GradientStyleType, SaveFormat } = AsposeCells;
//Instantiate the License class
var license = new License();
license.setLicense(data);
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
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```
## Constructors
| Name | Description |
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
