##Trendline
Represents a trendline in a chart.
## Trendline class
Represents a trendline in a chart.
```javascript
class Trendline extends Line;
```
### Example
```javascript
const { Workbook, ChartType, TrendlineType } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Excel object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.cells.get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.cells.get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").putValue("Y2");
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.nSeries.add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.nSeries.categoryData = "C1:C4";
//adding a linear trendline
var index = chart.nSeries.get(0).trendLines.add(TrendlineType.Linear);
var trendline = chart.nSeries.get(0).trendLines.get(index);
//Setting the custom name of the trendline.
trendline.name = "Linear";
//Displaying the equation on chart
trendline.displayEquation = true;
//Displaying the R-Squared value on chart
trendline.displayRSquared = true;
//Saving the Excel file
workbook.save("output/ChartsTrendline.xls");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Line)](#constructor-line-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isNameAuto](#isNameAuto--)| boolean | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [type](#type--)| TrendlineType | Readonly. Returns the trendline type. |
| [name](#name--)| string | Returns the name of the trendline. |
| [order](#order--)| number | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [period](#period--)| number | Returns or sets the period for the moving-average trendline. |
| [forward](#forward--)| number | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [backward](#backward--)| number | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [displayEquation](#displayEquation--)| boolean | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [displayRSquared](#displayRSquared--)| boolean | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [intercept](#intercept--)| number | Returns or sets the point where the trendline crosses the value axis. |
| [dataLabels](#dataLabels--)| DataLabels | Readonly. Represents the DataLabels object for the specified series. |
| [legendEntry](#legendEntry--)| LegendEntry | Readonly. Gets the legend entry according to this trendline |
| [compoundType](#compoundType--)| MsoLineStyle | Specifies the compound line type |
| [dashType](#dashType--)| MsoLineDashStyle | Specifies the dash line type |
| [capType](#capType--)| LineCapType | Specifies the ending caps. |
| [joinType](#joinType--)| LineJoinType | Specifies the joining caps. |
| [beginType](#beginType--)| MsoArrowheadStyle | Specifies an arrowhead for the begin of a line. |
| [endType](#endType--)| MsoArrowheadStyle | Specifies an arrowhead for the end of a line. |
| [beginArrowLength](#beginArrowLength--)| MsoArrowheadLength | Specifies the length of the arrowhead for the begin of a line. |
| [endArrowLength](#endArrowLength--)| MsoArrowheadLength | Specifies the length of the arrowhead for the end of a line. |
| [beginArrowWidth](#beginArrowWidth--)| MsoArrowheadWidth | Specifies the width of the arrowhead for the begin of a line. |
| [endArrowWidth](#endArrowWidth--)| MsoArrowheadWidth | Specifies the width of the arrowhead for the end of a line. |
| [themeColor](#themeColor--)| ThemeColor | Gets and sets the theme color. |
| [color](#color--)| Color | Represents the [Color](../color/) of the line. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [style](#style--)| LineType | Represents the style of the line. |
| [weight](#weight--)| WeightType | Gets or sets the [WeightType](../weighttype/) of the line. |
| [weightPt](#weightPt--)| number | Gets or sets the weight of the line in unit of points. |
| [weightPx](#weightPx--)| number | Gets or sets the weight of the line in unit of pixels. |
| [formattingType](#formattingType--)| ChartLineFormattingType | Gets or sets format type. |
| [isAutomaticColor](#isAutomaticColor--)| boolean | Readonly. Indicates whether the color of line is automatic assigned. |
| [isVisible](#isVisible--)| boolean | Represents whether the line is visible. |
| [isAuto](#isAuto--)| boolean | Indicates whether this line style is auto assigned. |
| [gradientFill](#gradientFill--)| GradientFill | Readonly. Represents gradient fill. |
## Methods
| Method | Description |
| --- | --- |
| [isNameAuto()](#isNameAuto--)| <b>@deprecated.</b> Please use the 'isNameAuto' property instead. Returns if Microsoft Excel automatically determines the name of the trendline. |
| [setIsNameAuto(boolean)](#setIsNameAuto-boolean-)| <b>@deprecated.</b> Please use the 'isNameAuto' property instead. Returns if Microsoft Excel automatically determines the name of the trendline. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Returns the trendline type. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns the name of the trendline. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Returns the name of the trendline. |
| [getOrder()](#getOrder--)| <b>@deprecated.</b> Please use the 'order' property instead. Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [setOrder(number)](#setOrder-number-)| <b>@deprecated.</b> Please use the 'order' property instead. Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [getPeriod()](#getPeriod--)| <b>@deprecated.</b> Please use the 'period' property instead. Returns or sets the period for the moving-average trendline. |
| [setPeriod(number)](#setPeriod-number-)| <b>@deprecated.</b> Please use the 'period' property instead. Returns or sets the period for the moving-average trendline. |
| [getForward()](#getForward--)| <b>@deprecated.</b> Please use the 'forward' property instead. Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [setForward(number)](#setForward-number-)| <b>@deprecated.</b> Please use the 'forward' property instead. Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [getBackward()](#getBackward--)| <b>@deprecated.</b> Please use the 'backward' property instead. Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [setBackward(number)](#setBackward-number-)| <b>@deprecated.</b> Please use the 'backward' property instead. Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [getDisplayEquation()](#getDisplayEquation--)| <b>@deprecated.</b> Please use the 'displayEquation' property instead. Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [setDisplayEquation(boolean)](#setDisplayEquation-boolean-)| <b>@deprecated.</b> Please use the 'displayEquation' property instead. Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [getDisplayRSquared()](#getDisplayRSquared--)| <b>@deprecated.</b> Please use the 'displayRSquared' property instead. Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [setDisplayRSquared(boolean)](#setDisplayRSquared-boolean-)| <b>@deprecated.</b> Please use the 'displayRSquared' property instead. Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [getIntercept()](#getIntercept--)| <b>@deprecated.</b> Please use the 'intercept' property instead. Returns or sets the point where the trendline crosses the value axis. |
| [setIntercept(number)](#setIntercept-number-)| <b>@deprecated.</b> Please use the 'intercept' property instead. Returns or sets the point where the trendline crosses the value axis. |
| [getDataLabels()](#getDataLabels--)| <b>@deprecated.</b> Please use the 'dataLabels' property instead. Represents the DataLabels object for the specified series. |
| [getLegendEntry()](#getLegendEntry--)| <b>@deprecated.</b> Please use the 'legendEntry' property instead. Gets the legend entry according to this trendline |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCompoundType()](#getCompoundType--)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the compound line type |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the compound line type |
| [getDashType()](#getDashType--)| <b>@deprecated.</b> Please use the 'dashType' property instead. Specifies the dash line type |
| [setDashType(MsoLineDashStyle)](#setDashType-msolinedashstyle-)| <b>@deprecated.</b> Please use the 'dashType' property instead. Specifies the dash line type |
| [getCapType()](#getCapType--)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the joining caps. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the joining caps. |
| [getBeginType()](#getBeginType--)| <b>@deprecated.</b> Please use the 'beginType' property instead. Specifies an arrowhead for the begin of a line. |
| [setBeginType(MsoArrowheadStyle)](#setBeginType-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'beginType' property instead. Specifies an arrowhead for the begin of a line. |
| [getEndType()](#getEndType--)| <b>@deprecated.</b> Please use the 'endType' property instead. Specifies an arrowhead for the end of a line. |
| [setEndType(MsoArrowheadStyle)](#setEndType-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'endType' property instead. Specifies an arrowhead for the end of a line. |
| [getBeginArrowLength()](#getBeginArrowLength--)| <b>@deprecated.</b> Please use the 'beginArrowLength' property instead. Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowLength(MsoArrowheadLength)](#setBeginArrowLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'beginArrowLength' property instead. Specifies the length of the arrowhead for the begin of a line. |
| [getEndArrowLength()](#getEndArrowLength--)| <b>@deprecated.</b> Please use the 'endArrowLength' property instead. Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowLength(MsoArrowheadLength)](#setEndArrowLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'endArrowLength' property instead. Specifies the length of the arrowhead for the end of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--)| <b>@deprecated.</b> Please use the 'beginArrowWidth' property instead. Specifies the width of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(MsoArrowheadWidth)](#setBeginArrowWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'beginArrowWidth' property instead. Specifies the width of the arrowhead for the begin of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--)| <b>@deprecated.</b> Please use the 'endArrowWidth' property instead. Specifies the width of the arrowhead for the end of a line. |
| [setEndArrowWidth(MsoArrowheadWidth)](#setEndArrowWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'endArrowWidth' property instead. Specifies the width of the arrowhead for the end of a line. |
| [getThemeColor()](#getThemeColor--)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Represents the [Color](../color/) of the line. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Represents the [Color](../color/) of the line. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getStyle()](#getStyle--)| <b>@deprecated.</b> Please use the 'style' property instead. Represents the style of the line. |
| [setStyle(LineType)](#setStyle-linetype-)| <b>@deprecated.</b> Please use the 'style' property instead. Represents the style of the line. |
| [getWeight()](#getWeight--)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the [WeightType](../weighttype/) of the line. |
| [setWeight(WeightType)](#setWeight-weighttype-)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the [WeightType](../weighttype/) of the line. |
| [getWeightPt()](#getWeightPt--)| <b>@deprecated.</b> Please use the 'weightPt' property instead. Gets or sets the weight of the line in unit of points. |
| [setWeightPt(number)](#setWeightPt-number-)| <b>@deprecated.</b> Please use the 'weightPt' property instead. Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--)| <b>@deprecated.</b> Please use the 'weightPx' property instead. Gets or sets the weight of the line in unit of pixels. |
| [setWeightPx(number)](#setWeightPx-number-)| <b>@deprecated.</b> Please use the 'weightPx' property instead. Gets or sets the weight of the line in unit of pixels. |
| [getFormattingType()](#getFormattingType--)| <b>@deprecated.</b> Please use the 'formattingType' property instead. Gets or sets format type. |
| [setFormattingType(ChartLineFormattingType)](#setFormattingType-chartlineformattingtype-)| <b>@deprecated.</b> Please use the 'formattingType' property instead. Gets or sets format type. |
| [isAutomaticColor()](#isAutomaticColor--)| <b>@deprecated.</b> Please use the 'isAutomaticColor' property instead. Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents whether the line is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents whether the line is visible. |
| [isAuto()](#isAuto--)| <b>@deprecated.</b> Please use the 'isAuto' property instead. Indicates whether this line style is auto assigned. |
| [setIsAuto(boolean)](#setIsAuto-boolean-)| <b>@deprecated.</b> Please use the 'isAuto' property instead. Indicates whether this line style is auto assigned. |
| [getGradientFill()](#getGradientFill--)| <b>@deprecated.</b> Please use the 'gradientFill' property instead. Represents gradient fill. |
### constructor(Line) {#constructor-line-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Line);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Line | The parent object. |
### isNameAuto {#isNameAuto--}
Returns if Microsoft Excel automatically determines the name of the trendline.
```javascript
isNameAuto : boolean;
```
### type {#type--}
Readonly. Returns the trendline type.
```javascript
type : TrendlineType;
```
### name {#name--}
Returns the name of the trendline.
```javascript
name : string;
```
### order {#order--}
Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.
```javascript
order : number;
```
### period {#period--}
Returns or sets the period for the moving-average trendline.
```javascript
period : number;
```
**Remarks**
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
### forward {#forward--}
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.
```javascript
forward : number;
```
### backward {#backward--}
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5
```javascript
backward : number;
```
### displayEquation {#displayEquation--}
Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.
```javascript
displayEquation : boolean;
```
### displayRSquared {#displayRSquared--}
Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.
```javascript
displayRSquared : boolean;
```
### intercept {#intercept--}
Returns or sets the point where the trendline crosses the value axis.
```javascript
intercept : number;
```
### dataLabels {#dataLabels--}
Readonly. Represents the DataLabels object for the specified series.
```javascript
dataLabels : DataLabels;
```
### legendEntry {#legendEntry--}
Readonly. Gets the legend entry according to this trendline
```javascript
legendEntry : LegendEntry;
```
### compoundType {#compoundType--}
Specifies the compound line type
```javascript
compoundType : MsoLineStyle;
```
### dashType {#dashType--}
Specifies the dash line type
```javascript
dashType : MsoLineDashStyle;
```
### capType {#capType--}
Specifies the ending caps.
```javascript
capType : LineCapType;
```
### joinType {#joinType--}
Specifies the joining caps.
```javascript
joinType : LineJoinType;
```
### beginType {#beginType--}
Specifies an arrowhead for the begin of a line.
```javascript
beginType : MsoArrowheadStyle;
```
### endType {#endType--}
Specifies an arrowhead for the end of a line.
```javascript
endType : MsoArrowheadStyle;
```
### beginArrowLength {#beginArrowLength--}
Specifies the length of the arrowhead for the begin of a line.
```javascript
beginArrowLength : MsoArrowheadLength;
```
### endArrowLength {#endArrowLength--}
Specifies the length of the arrowhead for the end of a line.
```javascript
endArrowLength : MsoArrowheadLength;
```
### beginArrowWidth {#beginArrowWidth--}
Specifies the width of the arrowhead for the begin of a line.
```javascript
beginArrowWidth : MsoArrowheadWidth;
```
### endArrowWidth {#endArrowWidth--}
Specifies the width of the arrowhead for the end of a line.
```javascript
endArrowWidth : MsoArrowheadWidth;
```
### themeColor {#themeColor--}
Gets and sets the theme color.
```javascript
themeColor : ThemeColor;
```
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
### color {#color--}
Represents the [Color](../color/) of the line.
```javascript
color : Color;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### style {#style--}
Represents the style of the line.
```javascript
style : LineType;
```
### weight {#weight--}
Gets or sets the [WeightType](../weighttype/) of the line.
```javascript
weight : WeightType;
```
### weightPt {#weightPt--}
Gets or sets the weight of the line in unit of points.
```javascript
weightPt : number;
```
### weightPx {#weightPx--}
Gets or sets the weight of the line in unit of pixels.
```javascript
weightPx : number;
```
### formattingType {#formattingType--}
Gets or sets format type.
```javascript
formattingType : ChartLineFormattingType;
```
### isAutomaticColor {#isAutomaticColor--}
Readonly. Indicates whether the color of line is automatic assigned.
```javascript
isAutomaticColor : boolean;
```
### isVisible {#isVisible--}
Represents whether the line is visible.
```javascript
isVisible : boolean;
```
### isAuto {#isAuto--}
Indicates whether this line style is auto assigned.
```javascript
isAuto : boolean;
```
### gradientFill {#gradientFill--}
Readonly. Represents gradient fill.
```javascript
gradientFill : GradientFill;
```
### isNameAuto() {#isNameAuto--}
```javascript
isNameAuto() : boolean;
```
### setIsNameAuto(boolean) {#setIsNameAuto-boolean-}
```javascript
setIsNameAuto(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getType() {#getType--}
```javascript
getType() : TrendlineType;
```
**Returns**
[TrendlineType](../trendlinetype/)
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getOrder() {#getOrder--}
```javascript
getOrder() : number;
```
### setOrder(number) {#setOrder-number-}
```javascript
setOrder(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPeriod() {#getPeriod--}
```javascript
getPeriod() : number;
```
**Remarks**
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
### setPeriod(number) {#setPeriod-number-}
```javascript
setPeriod(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
### getForward() {#getForward--}
```javascript
getForward() : number;
```
### setForward(number) {#setForward-number-}
```javascript
setForward(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBackward() {#getBackward--}
```javascript
getBackward() : number;
```
### setBackward(number) {#setBackward-number-}
```javascript
setBackward(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDisplayEquation() {#getDisplayEquation--}
```javascript
getDisplayEquation() : boolean;
```
### setDisplayEquation(boolean) {#setDisplayEquation-boolean-}
```javascript
setDisplayEquation(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDisplayRSquared() {#getDisplayRSquared--}
```javascript
getDisplayRSquared() : boolean;
```
### setDisplayRSquared(boolean) {#setDisplayRSquared-boolean-}
```javascript
setDisplayRSquared(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIntercept() {#getIntercept--}
```javascript
getIntercept() : number;
```
### setIntercept(number) {#setIntercept-number-}
```javascript
setIntercept(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDataLabels() {#getDataLabels--}
```javascript
getDataLabels() : DataLabels;
```
**Returns**
[DataLabels](../datalabels/)
### getLegendEntry() {#getLegendEntry--}
```javascript
getLegendEntry() : LegendEntry;
```
**Returns**
[LegendEntry](../legendentry/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getCompoundType() {#getCompoundType--}
```javascript
getCompoundType() : MsoLineStyle;
```
**Returns**
[MsoLineStyle](../msolinestyle/)
### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}
```javascript
setCompoundType(value: MsoLineStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |
### getDashType() {#getDashType--}
```javascript
getDashType() : MsoLineDashStyle;
```
**Returns**
[MsoLineDashStyle](../msolinedashstyle/)
### setDashType(MsoLineDashStyle) {#setDashType-msolinedashstyle-}
```javascript
setDashType(value: MsoLineDashStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |
### getCapType() {#getCapType--}
```javascript
getCapType() : LineCapType;
```
**Returns**
[LineCapType](../linecaptype/)
### setCapType(LineCapType) {#setCapType-linecaptype-}
```javascript
setCapType(value: LineCapType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |
### getJoinType() {#getJoinType--}
```javascript
getJoinType() : LineJoinType;
```
**Returns**
[LineJoinType](../linejointype/)
### setJoinType(LineJoinType) {#setJoinType-linejointype-}
```javascript
setJoinType(value: LineJoinType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |
### getBeginType() {#getBeginType--}
```javascript
getBeginType() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setBeginType(MsoArrowheadStyle) {#setBeginType-msoarrowheadstyle-}
```javascript
setBeginType(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getEndType() {#getEndType--}
```javascript
getEndType() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setEndType(MsoArrowheadStyle) {#setEndType-msoarrowheadstyle-}
```javascript
setEndType(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getBeginArrowLength() {#getBeginArrowLength--}
```javascript
getBeginArrowLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setBeginArrowLength(MsoArrowheadLength) {#setBeginArrowLength-msoarrowheadlength-}
```javascript
setBeginArrowLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getEndArrowLength() {#getEndArrowLength--}
```javascript
getEndArrowLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setEndArrowLength(MsoArrowheadLength) {#setEndArrowLength-msoarrowheadlength-}
```javascript
setEndArrowLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getBeginArrowWidth() {#getBeginArrowWidth--}
```javascript
getBeginArrowWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setBeginArrowWidth(MsoArrowheadWidth) {#setBeginArrowWidth-msoarrowheadwidth-}
```javascript
setBeginArrowWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getEndArrowWidth() {#getEndArrowWidth--}
```javascript
getEndArrowWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setEndArrowWidth(MsoArrowheadWidth) {#setEndArrowWidth-msoarrowheadwidth-}
```javascript
setEndArrowWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getThemeColor() {#getThemeColor--}
```javascript
getThemeColor() : ThemeColor;
```
**Returns**
[ThemeColor](../themecolor/)
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}
```javascript
setThemeColor(value: ThemeColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
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
### getStyle() {#getStyle--}
```javascript
getStyle() : LineType;
```
**Returns**
[LineType](../linetype/)
### setStyle(LineType) {#setStyle-linetype-}
```javascript
setStyle(value: LineType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineType](../linetype/) | The value to set. |
### getWeight() {#getWeight--}
```javascript
getWeight() : WeightType;
```
**Returns**
[WeightType](../weighttype/)
### setWeight(WeightType) {#setWeight-weighttype-}
```javascript
setWeight(value: WeightType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WeightType](../weighttype/) | The value to set. |
### getWeightPt() {#getWeightPt--}
```javascript
getWeightPt() : number;
```
### setWeightPt(number) {#setWeightPt-number-}
```javascript
setWeightPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWeightPx() {#getWeightPx--}
```javascript
getWeightPx() : number;
```
### setWeightPx(number) {#setWeightPx-number-}
```javascript
setWeightPx(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFormattingType() {#getFormattingType--}
```javascript
getFormattingType() : ChartLineFormattingType;
```
**Returns**
[ChartLineFormattingType](../chartlineformattingtype/)
### setFormattingType(ChartLineFormattingType) {#setFormattingType-chartlineformattingtype-}
```javascript
setFormattingType(value: ChartLineFormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartLineFormattingType](../chartlineformattingtype/) | The value to set. |
### isAutomaticColor() {#isAutomaticColor--}
```javascript
isAutomaticColor() : boolean;
```
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isAuto() {#isAuto--}
```javascript
isAuto() : boolean;
```
### setIsAuto(boolean) {#setIsAuto-boolean-}
```javascript
setIsAuto(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getGradientFill() {#getGradientFill--}
```javascript
getGradientFill() : GradientFill;
```
**Returns**
[GradientFill](../gradientfill/)
