##ChartDataTable
Represents a chart data table.
## ChartDataTable class
Represents a chart data table.
```javascript
class ChartDataTable;
```
### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the first worksheet
var worksheet = workbook.worksheets.get(0);
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
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.nSeries.add("A1:B3", true);
chart.showDataTable = true;
//Getting Chart Table
var chartTable = chart.getChartDataTable();
//Setting Chart Table Font Color
chartTable.font.color = Color.Red;
//Setting Legend Key Visibility
chartTable.showLegendKey = false;
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [font](#font--)| Font | Readonly. Gets a [Font](../font/) object which represents the font setting of the specified chart data table. |
| [autoScaleFont](#autoScaleFont--)| boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [hasBorderHorizontal](#hasBorderHorizontal--)| boolean | True if the chart data table has horizontal cell borders |
| [hasHorizontalBorder](#hasHorizontalBorder--)| boolean | True if the chart data table has horizontal cell borders |
| [hasBorderVertical](#hasBorderVertical--)| boolean | True if the chart data table has vertical cell borders |
| [hasVerticalBorder](#hasVerticalBorder--)| boolean | True if the chart data table has vertical cell borders |
| [hasBorderOutline](#hasBorderOutline--)| boolean | True if the chart data table has outline borders |
| [hasOutlineBorder](#hasOutlineBorder--)| boolean | True if the chart data table has outline borders |
| [showLegendKey](#showLegendKey--)| boolean | True if the data label legend key is visible. |
| [border](#border--)| Line | Readonly. Returns a Border object that represents the border of the object |
### font {#font--}
Readonly. Gets a [Font](../font/) object which represents the font setting of the specified chart data table.
```javascript
font : Font;
```
### autoScaleFont {#autoScaleFont--}
True if the text in the object changes font size when the object size changes. The default value is True.
```javascript
autoScaleFont : boolean;
```
### backgroundMode {#backgroundMode--}
Gets and sets the display mode of the background
```javascript
backgroundMode : BackgroundMode;
```
### hasBorderHorizontal {#hasBorderHorizontal--}
True if the chart data table has horizontal cell borders
```javascript
hasBorderHorizontal : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### hasHorizontalBorder {#hasHorizontalBorder--}
True if the chart data table has horizontal cell borders
```javascript
hasHorizontalBorder : boolean;
```
### hasBorderVertical {#hasBorderVertical--}
True if the chart data table has vertical cell borders
```javascript
hasBorderVertical : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### hasVerticalBorder {#hasVerticalBorder--}
True if the chart data table has vertical cell borders
```javascript
hasVerticalBorder : boolean;
```
### hasBorderOutline {#hasBorderOutline--}
True if the chart data table has outline borders
```javascript
hasBorderOutline : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### hasOutlineBorder {#hasOutlineBorder--}
True if the chart data table has outline borders
```javascript
hasOutlineBorder : boolean;
```
### showLegendKey {#showLegendKey--}
True if the data label legend key is visible.
```javascript
showLegendKey : boolean;
```
### border {#border--}
Readonly. Returns a Border object that represents the border of the object
```javascript
border : Line;
```
