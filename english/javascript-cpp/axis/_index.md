---
title: Axis
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an axis of chart.
type: docs
url: /javascript-cpp/axis/
---

## Axis class

Encapsulates the object that represents an axis of chart.

```javascript
class Axis;
```


### Example
```javascript
const { Workbook, ChartType, CrossType, SaveFormat } = AsposeCells;

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
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(4);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(20);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.nSeries.add("A1:B3", true);
//Set the max value of value axis
chart.valueAxis.maxValue = 200;
//Set the min value of value axis
chart.valueAxis.minValue = 0;
//Set the major unit
chart.valueAxis.majorUnit = 25;
//Category(X) axis crosses at the maxinum value.
chart.valueAxis.crossType = CrossType.Maximum;
//Set he number of categories or series between tick-mark labels. 
chart.categoryAxis.tickLabelSpacing = 2;
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [area](#area--)| Area | Readonly. Gets the [Area](../area/). |
| [isAutomaticMinValue](#isAutomaticMinValue--)| boolean | Indicates whether the min value is automatically assigned. |
| [minValue](#minValue--)| VObject | Represents the minimum value on the value axis. |
| [isAutomaticMaxValue](#isAutomaticMaxValue--)| boolean | Indicates whether the max value is automatically assigned. |
| [maxValue](#maxValue--)| VObject | Represents the maximum value on the value axis. |
| [isAutomaticMajorUnit](#isAutomaticMajorUnit--)| boolean | Indicates whether the major unit of the axis is automatically assigned. |
| [majorUnit](#majorUnit--)| number | Represents the major units for the axis. |
| [isAutomaticMinorUnit](#isAutomaticMinorUnit--)| boolean | Indicates whether the minor unit of the axis is automatically assigned. |
| [minorUnit](#minorUnit--)| number | Represents the minor units for the axis. |
| [axisLine](#axisLine--)| Line | Readonly. Gets the appearance of an Axis. |
| [majorTickMark](#majorTickMark--)| TickMarkType | Represents the type of major tick mark for the specified axis. |
| [minorTickMark](#minorTickMark--)| TickMarkType | Represents the type of minor tick mark for the specified axis. |
| [tickLabelPosition](#tickLabelPosition--)| TickLabelPositionType | Represents the position of tick-mark labels on the specified axis. |
| [crossAt](#crossAt--)| number | Represents the point on the value axis where the category axis crosses it. |
| [crossType](#crossType--)| CrossType | Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [logBase](#logBase--)| number | Represents the logarithmic base. Default value is 10. |
| [isLogarithmic](#isLogarithmic--)| boolean | Represents if the value axis scale type is logarithmic or not. |
| [isPlotOrderReversed](#isPlotOrderReversed--)| boolean | Represents if Microsoft Excel plots data points from last to first. |
| [axisBetweenCategories](#axisBetweenCategories--)| boolean | Represents if the value axis crosses the category axis between categories. |
| [tickLabels](#tickLabels--)| TickLabels | Readonly. Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis. |
| [tickLabelSpacing](#tickLabelSpacing--)| number | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [isAutoTickLabelSpacing](#isAutoTickLabelSpacing--)| boolean | Indicates whether the spacing of tick label is automatic |
| [tickMarkSpacing](#tickMarkSpacing--)| number | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [displayUnit](#displayUnit--)| DisplayUnitType | Represents the unit label for the specified axis. |
| [customUnit](#customUnit--)| number | Specifies a custom value for the display unit. |
| [customDisplayUnit](#customDisplayUnit--)| number | Specifies a custom value for the display unit. |
| [displayUnitLabel](#displayUnitLabel--)| DisplayUnitLabel | Readonly. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [isDisplayUnitLabelShown](#isDisplayUnitLabelShown--)| boolean | Represents if the display unit label is shown on the specified axis. |
| [title](#title--)| Title | Readonly. Gets the title of this axis in the chart. |
| [categoryType](#categoryType--)| CategoryType | Represents the type of the category axis. |
| [baseUnitScale](#baseUnitScale--)| TimeUnit | Represents the base unit scale for the category axis. |
| [majorUnitScale](#majorUnitScale--)| TimeUnit | Represents the major unit scale for the category axis. |
| [minorUnitScale](#minorUnitScale--)| TimeUnit | Represents the major unit scale for the category axis. |
| [isVisible](#isVisible--)| boolean | Represents if the axis is visible. |
| [majorGridLines](#majorGridLines--)| Line | Readonly. Represents major gridlines on a chart axis. |
| [minorGridLines](#minorGridLines--)| Line | Readonly. Represents minor gridlines on a chart axis. |
| [hasMultiLevelLabels](#hasMultiLevelLabels--)| boolean | Indicates whether the labels shall be shown as multi level. |
| [bins](#bins--)| AxisBins | Readonly. Represents bins on a chart(Histogram/Pareto) axis |

## Methods

| Method | Description |
| --- | --- |
| [getAxisTexts()](#getAxisTexts--)| Gets the labels of the axis after call Chart.Calculate() method. |


### area {#area--}

Readonly. Gets the [Area](../area/).

```javascript
area : Area;
```


### isAutomaticMinValue {#isAutomaticMinValue--}

Indicates whether the min value is automatically assigned.

```javascript
isAutomaticMinValue : boolean;
```


### minValue {#minValue--}

Represents the minimum value on the value axis.

```javascript
minValue : VObject;
```


**Remarks**

The minValue type only can be double or DateTime

### isAutomaticMaxValue {#isAutomaticMaxValue--}

Indicates whether the max value is automatically assigned.

```javascript
isAutomaticMaxValue : boolean;
```


### maxValue {#maxValue--}

Represents the maximum value on the value axis.

```javascript
maxValue : VObject;
```


**Remarks**

The maxValue type only can be double or DateTime

### isAutomaticMajorUnit {#isAutomaticMajorUnit--}

Indicates whether the major unit of the axis is automatically assigned.

```javascript
isAutomaticMajorUnit : boolean;
```


### majorUnit {#majorUnit--}

Represents the major units for the axis.

```javascript
majorUnit : number;
```


**Remarks**

The major units must be greater than zero.

### isAutomaticMinorUnit {#isAutomaticMinorUnit--}

Indicates whether the minor unit of the axis is automatically assigned.

```javascript
isAutomaticMinorUnit : boolean;
```


### minorUnit {#minorUnit--}

Represents the minor units for the axis.

```javascript
minorUnit : number;
```


**Remarks**

The minor units must be greater than zero.

### axisLine {#axisLine--}

Readonly. Gets the appearance of an Axis.

```javascript
axisLine : Line;
```


### majorTickMark {#majorTickMark--}

Represents the type of major tick mark for the specified axis.

```javascript
majorTickMark : TickMarkType;
```


### minorTickMark {#minorTickMark--}

Represents the type of minor tick mark for the specified axis.

```javascript
minorTickMark : TickMarkType;
```


### tickLabelPosition {#tickLabelPosition--}

Represents the position of tick-mark labels on the specified axis.

```javascript
tickLabelPosition : TickLabelPositionType;
```


### crossAt {#crossAt--}

Represents the point on the value axis where the category axis crosses it.

```javascript
crossAt : number;
```


**Remarks**

The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### crossType {#crossType--}

Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses.

```javascript
crossType : CrossType;
```


### logBase {#logBase--}

Represents the logarithmic base. Default value is 10.

```javascript
logBase : number;
```


### isLogarithmic {#isLogarithmic--}

Represents if the value axis scale type is logarithmic or not.

```javascript
isLogarithmic : boolean;
```


### isPlotOrderReversed {#isPlotOrderReversed--}

Represents if Microsoft Excel plots data points from last to first.

```javascript
isPlotOrderReversed : boolean;
```


### axisBetweenCategories {#axisBetweenCategories--}

Represents if the value axis crosses the category axis between categories.

```javascript
axisBetweenCategories : boolean;
```


**Remarks**

This property applies only to category axes, and it doesn't apply to 3-D charts.

### tickLabels {#tickLabels--}

Readonly. Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis.

```javascript
tickLabels : TickLabels;
```


### tickLabelSpacing {#tickLabelSpacing--}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.

```javascript
tickLabelSpacing : number;
```


**Remarks**

The number must be between 1 and 31999.

### isAutoTickLabelSpacing {#isAutoTickLabelSpacing--}

Indicates whether the spacing of tick label is automatic

```javascript
isAutoTickLabelSpacing : boolean;
```


### tickMarkSpacing {#tickMarkSpacing--}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes.

```javascript
tickMarkSpacing : number;
```


**Remarks**

The number must be between 1 and 31999.

### displayUnit {#displayUnit--}

Represents the unit label for the specified axis.

```javascript
displayUnit : DisplayUnitType;
```


### customUnit {#customUnit--}

Specifies a custom value for the display unit.

```javascript
customUnit : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use Axis.CustomDisplayUnit property. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### customDisplayUnit {#customDisplayUnit--}

Specifies a custom value for the display unit.

```javascript
customDisplayUnit : number;
```


### displayUnitLabel {#displayUnitLabel--}

Readonly. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

```javascript
displayUnitLabel : DisplayUnitLabel;
```


### isDisplayUnitLabelShown {#isDisplayUnitLabelShown--}

Represents if the display unit label is shown on the specified axis.

```javascript
isDisplayUnitLabelShown : boolean;
```


**Remarks**

The default value is True.

### title {#title--}

Readonly. Gets the title of this axis in the chart.

```javascript
title : Title;
```


### categoryType {#categoryType--}

Represents the type of the category axis.

```javascript
categoryType : CategoryType;
```


### baseUnitScale {#baseUnitScale--}

Represents the base unit scale for the category axis.

```javascript
baseUnitScale : TimeUnit;
```


**Remarks**

Setting this property only takes effect when the CategoryType property is set to TimeScale.

### majorUnitScale {#majorUnitScale--}

Represents the major unit scale for the category axis.

```javascript
majorUnitScale : TimeUnit;
```


**Example**
```javascript
const { Workbook, ChartType, CategoryType, TimeUnit } = AsposeCells;

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
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(4);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(20);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);

//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
chart.categoryAxis.categoryType = CategoryType.TimeScale;
chart.categoryAxis.majorUnitScale = TimeUnit.Months;
chart.categoryAxis.majorUnit = 2;
```

### minorUnitScale {#minorUnitScale--}

Represents the major unit scale for the category axis.

```javascript
minorUnitScale : TimeUnit;
```


**Example**
```javascript
const { Workbook, ChartType, CategoryType, TimeUnit } = AsposeCells;

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
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(4);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(20);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);

//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
chart.categoryAxis.categoryType = CategoryType.TimeScale;
chart.categoryAxis.minorUnitScale = TimeUnit.Months;
chart.categoryAxis.minorUnit = 2;
```

### isVisible {#isVisible--}

Represents if the axis is visible.

```javascript
isVisible : boolean;
```


### majorGridLines {#majorGridLines--}

Readonly. Represents major gridlines on a chart axis.

```javascript
majorGridLines : Line;
```


**Example**
```javascript
const { Workbook, ChartType } = AsposeCells;

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
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(4);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(20);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);

//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
chart.valueAxis.majorGridLines.isVisible = false;
chart.categoryAxis.majorGridLines.isVisible = true;
```

### minorGridLines {#minorGridLines--}

Readonly. Represents minor gridlines on a chart axis.

```javascript
minorGridLines : Line;
```


### hasMultiLevelLabels {#hasMultiLevelLabels--}

Indicates whether the labels shall be shown as multi level.

```javascript
hasMultiLevelLabels : boolean;
```


**Remarks**

Only valid for category axis.

### bins {#bins--}

Readonly. Represents bins on a chart(Histogram/Pareto) axis

```javascript
bins : AxisBins;
```


### getAxisTexts() {#getAxisTexts--}

Gets the labels of the axis after call Chart.Calculate() method.

```javascript
getAxisTexts() : string[];
```


**Returns**

string[]


