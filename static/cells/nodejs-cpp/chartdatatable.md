##ChartDataTable
Represents a chart data table.
## ChartDataTable class
Represents a chart data table.
```javascript
class ChartDataTable;
```
### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");
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
workbook.save("output/ChartsChartDataTable.xls");
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
## Methods
| Method | Description |
| --- | --- |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Gets a [Font](../font/) object which represents the font setting of the specified chart data table. |
| [getAutoScaleFont()](#getAutoScaleFont--)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackgroundMode()](#getBackgroundMode--)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [getHasBorderHorizontal()](#getHasBorderHorizontal--)| <b>@deprecated.</b> Please use the 'hasBorderHorizontal' property instead. True if the chart data table has horizontal cell borders |
| [setHasBorderHorizontal(boolean)](#setHasBorderHorizontal-boolean-)| <b>@deprecated.</b> Please use the 'hasBorderHorizontal' property instead. True if the chart data table has horizontal cell borders |
| [getHasHorizontalBorder()](#getHasHorizontalBorder--)| <b>@deprecated.</b> Please use the 'hasHorizontalBorder' property instead. True if the chart data table has horizontal cell borders |
| [setHasHorizontalBorder(boolean)](#setHasHorizontalBorder-boolean-)| <b>@deprecated.</b> Please use the 'hasHorizontalBorder' property instead. True if the chart data table has horizontal cell borders |
| [getHasBorderVertical()](#getHasBorderVertical--)| <b>@deprecated.</b> Please use the 'hasBorderVertical' property instead. True if the chart data table has vertical cell borders |
| [setHasBorderVertical(boolean)](#setHasBorderVertical-boolean-)| <b>@deprecated.</b> Please use the 'hasBorderVertical' property instead. True if the chart data table has vertical cell borders |
| [getHasVerticalBorder()](#getHasVerticalBorder--)| <b>@deprecated.</b> Please use the 'hasVerticalBorder' property instead. True if the chart data table has vertical cell borders |
| [setHasVerticalBorder(boolean)](#setHasVerticalBorder-boolean-)| <b>@deprecated.</b> Please use the 'hasVerticalBorder' property instead. True if the chart data table has vertical cell borders |
| [getHasBorderOutline()](#getHasBorderOutline--)| <b>@deprecated.</b> Please use the 'hasBorderOutline' property instead. True if the chart data table has outline borders |
| [setHasBorderOutline(boolean)](#setHasBorderOutline-boolean-)| <b>@deprecated.</b> Please use the 'hasBorderOutline' property instead. True if the chart data table has outline borders |
| [getHasOutlineBorder()](#getHasOutlineBorder--)| <b>@deprecated.</b> Please use the 'hasOutlineBorder' property instead. True if the chart data table has outline borders |
| [setHasOutlineBorder(boolean)](#setHasOutlineBorder-boolean-)| <b>@deprecated.</b> Please use the 'hasOutlineBorder' property instead. True if the chart data table has outline borders |
| [getShowLegendKey()](#getShowLegendKey--)| <b>@deprecated.</b> Please use the 'showLegendKey' property instead. True if the data label legend key is visible. |
| [setShowLegendKey(boolean)](#setShowLegendKey-boolean-)| <b>@deprecated.</b> Please use the 'showLegendKey' property instead. True if the data label legend key is visible. |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Returns a Border object that represents the border of the object |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getAutoScaleFont() {#getAutoScaleFont--}
```javascript
getAutoScaleFont() : boolean;
```
### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}
```javascript
setAutoScaleFont(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBackgroundMode() {#getBackgroundMode--}
```javascript
getBackgroundMode() : BackgroundMode;
```
**Returns**
[BackgroundMode](../backgroundmode/)
### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}
```javascript
setBackgroundMode(value: BackgroundMode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |
### getHasBorderHorizontal() {#getHasBorderHorizontal--}
```javascript
getHasBorderHorizontal() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### setHasBorderHorizontal(boolean) {#setHasBorderHorizontal-boolean-}
```javascript
setHasBorderHorizontal(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### getHasHorizontalBorder() {#getHasHorizontalBorder--}
```javascript
getHasHorizontalBorder() : boolean;
```
### setHasHorizontalBorder(boolean) {#setHasHorizontalBorder-boolean-}
```javascript
setHasHorizontalBorder(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHasBorderVertical() {#getHasBorderVertical--}
```javascript
getHasBorderVertical() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### setHasBorderVertical(boolean) {#setHasBorderVertical-boolean-}
```javascript
setHasBorderVertical(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### getHasVerticalBorder() {#getHasVerticalBorder--}
```javascript
getHasVerticalBorder() : boolean;
```
### setHasVerticalBorder(boolean) {#setHasVerticalBorder-boolean-}
```javascript
setHasVerticalBorder(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHasBorderOutline() {#getHasBorderOutline--}
```javascript
getHasBorderOutline() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### setHasBorderOutline(boolean) {#setHasBorderOutline-boolean-}
```javascript
setHasBorderOutline(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### getHasOutlineBorder() {#getHasOutlineBorder--}
```javascript
getHasOutlineBorder() : boolean;
```
### setHasOutlineBorder(boolean) {#setHasOutlineBorder-boolean-}
```javascript
setHasOutlineBorder(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowLegendKey() {#getShowLegendKey--}
```javascript
getShowLegendKey() : boolean;
```
### setShowLegendKey(boolean) {#setShowLegendKey-boolean-}
```javascript
setShowLegendKey(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
