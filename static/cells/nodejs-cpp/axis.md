##Axis
Encapsulates the object that represents an axis of chart.
## Axis class
Encapsulates the object that represents an axis of chart.
```javascript
class Axis;
```
### Example
```javascript
const { Workbook, ChartType, CrossType } = require("aspose.cells.node");
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
workbook.save("output/ChartsAxis.xlsx");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [area](#area--)| Area | Readonly. Gets the [Area](../area/). |
| [isAutomaticMinValue](#isAutomaticMinValue--)| boolean | Indicates whether the min value is automatically assigned. |
| [minValue](#minValue--)| Object | Represents the minimum value on the value axis. |
| [isAutomaticMaxValue](#isAutomaticMaxValue--)| boolean | Indicates whether the max value is automatically assigned. |
| [maxValue](#maxValue--)| Object | Represents the maximum value on the value axis. |
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
| [logBase](#logBase--)| number | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
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
| [title](#title--)| Title | Readonly. Gets the axis' title. |
| [categoryType](#categoryType--)| CategoryType | Represents the category axis type. |
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
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Gets the [Area](../area/). |
| [isAutomaticMinValue()](#isAutomaticMinValue--)| <b>@deprecated.</b> Please use the 'isAutomaticMinValue' property instead. Indicates whether the min value is automatically assigned. |
| [setIsAutomaticMinValue(boolean)](#setIsAutomaticMinValue-boolean-)| <b>@deprecated.</b> Please use the 'isAutomaticMinValue' property instead. Indicates whether the min value is automatically assigned. |
| [getMinValue()](#getMinValue--)| <b>@deprecated.</b> Please use the 'minValue' property instead. Represents the minimum value on the value axis. |
| [setMinValue(Object)](#setMinValue-object-)| <b>@deprecated.</b> Please use the 'minValue' property instead. Represents the minimum value on the value axis. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--)| <b>@deprecated.</b> Please use the 'isAutomaticMaxValue' property instead. Indicates whether the max value is automatically assigned. |
| [setIsAutomaticMaxValue(boolean)](#setIsAutomaticMaxValue-boolean-)| <b>@deprecated.</b> Please use the 'isAutomaticMaxValue' property instead. Indicates whether the max value is automatically assigned. |
| [getMaxValue()](#getMaxValue--)| <b>@deprecated.</b> Please use the 'maxValue' property instead. Represents the maximum value on the value axis. |
| [setMaxValue(Object)](#setMaxValue-object-)| <b>@deprecated.</b> Please use the 'maxValue' property instead. Represents the maximum value on the value axis. |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--)| <b>@deprecated.</b> Please use the 'isAutomaticMajorUnit' property instead. Indicates whether the major unit of the axis is automatically assigned. |
| [setIsAutomaticMajorUnit(boolean)](#setIsAutomaticMajorUnit-boolean-)| <b>@deprecated.</b> Please use the 'isAutomaticMajorUnit' property instead. Indicates whether the major unit of the axis is automatically assigned. |
| [getMajorUnit()](#getMajorUnit--)| <b>@deprecated.</b> Please use the 'majorUnit' property instead. Represents the major units for the axis. |
| [setMajorUnit(number)](#setMajorUnit-number-)| <b>@deprecated.</b> Please use the 'majorUnit' property instead. Represents the major units for the axis. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--)| <b>@deprecated.</b> Please use the 'isAutomaticMinorUnit' property instead. Indicates whether the minor unit of the axis is automatically assigned. |
| [setIsAutomaticMinorUnit(boolean)](#setIsAutomaticMinorUnit-boolean-)| <b>@deprecated.</b> Please use the 'isAutomaticMinorUnit' property instead. Indicates whether the minor unit of the axis is automatically assigned. |
| [getMinorUnit()](#getMinorUnit--)| <b>@deprecated.</b> Please use the 'minorUnit' property instead. Represents the minor units for the axis. |
| [setMinorUnit(number)](#setMinorUnit-number-)| <b>@deprecated.</b> Please use the 'minorUnit' property instead. Represents the minor units for the axis. |
| [getAxisLine()](#getAxisLine--)| <b>@deprecated.</b> Please use the 'axisLine' property instead. Gets the appearance of an Axis. |
| [getMajorTickMark()](#getMajorTickMark--)| <b>@deprecated.</b> Please use the 'majorTickMark' property instead. Represents the type of major tick mark for the specified axis. |
| [setMajorTickMark(TickMarkType)](#setMajorTickMark-tickmarktype-)| <b>@deprecated.</b> Please use the 'majorTickMark' property instead. Represents the type of major tick mark for the specified axis. |
| [getMinorTickMark()](#getMinorTickMark--)| <b>@deprecated.</b> Please use the 'minorTickMark' property instead. Represents the type of minor tick mark for the specified axis. |
| [setMinorTickMark(TickMarkType)](#setMinorTickMark-tickmarktype-)| <b>@deprecated.</b> Please use the 'minorTickMark' property instead. Represents the type of minor tick mark for the specified axis. |
| [getTickLabelPosition()](#getTickLabelPosition--)| <b>@deprecated.</b> Please use the 'tickLabelPosition' property instead. Represents the position of tick-mark labels on the specified axis. |
| [setTickLabelPosition(TickLabelPositionType)](#setTickLabelPosition-ticklabelpositiontype-)| <b>@deprecated.</b> Please use the 'tickLabelPosition' property instead. Represents the position of tick-mark labels on the specified axis. |
| [getCrossAt()](#getCrossAt--)| <b>@deprecated.</b> Please use the 'crossAt' property instead. Represents the point on the value axis where the category axis crosses it. |
| [setCrossAt(number)](#setCrossAt-number-)| <b>@deprecated.</b> Please use the 'crossAt' property instead. Represents the point on the value axis where the category axis crosses it. |
| [getCrossType()](#getCrossType--)| <b>@deprecated.</b> Please use the 'crossType' property instead. Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [setCrossType(CrossType)](#setCrossType-crosstype-)| <b>@deprecated.</b> Please use the 'crossType' property instead. Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [getLogBase()](#getLogBase--)| <b>@deprecated.</b> Please use the 'logBase' property instead. Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [setLogBase(number)](#setLogBase-number-)| <b>@deprecated.</b> Please use the 'logBase' property instead. Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [isLogarithmic()](#isLogarithmic--)| <b>@deprecated.</b> Please use the 'isLogarithmic' property instead. Represents if the value axis scale type is logarithmic or not. |
| [setIsLogarithmic(boolean)](#setIsLogarithmic-boolean-)| <b>@deprecated.</b> Please use the 'isLogarithmic' property instead. Represents if the value axis scale type is logarithmic or not. |
| [isPlotOrderReversed()](#isPlotOrderReversed--)| <b>@deprecated.</b> Please use the 'isPlotOrderReversed' property instead. Represents if Microsoft Excel plots data points from last to first. |
| [setIsPlotOrderReversed(boolean)](#setIsPlotOrderReversed-boolean-)| <b>@deprecated.</b> Please use the 'isPlotOrderReversed' property instead. Represents if Microsoft Excel plots data points from last to first. |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--)| <b>@deprecated.</b> Please use the 'axisBetweenCategories' property instead. Represents if the value axis crosses the category axis between categories. |
| [setAxisBetweenCategories(boolean)](#setAxisBetweenCategories-boolean-)| <b>@deprecated.</b> Please use the 'axisBetweenCategories' property instead. Represents if the value axis crosses the category axis between categories. |
| [getTickLabels()](#getTickLabels--)| <b>@deprecated.</b> Please use the 'tickLabels' property instead. Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis. |
| [getTickLabelSpacing()](#getTickLabelSpacing--)| <b>@deprecated.</b> Please use the 'tickLabelSpacing' property instead. Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [setTickLabelSpacing(number)](#setTickLabelSpacing-number-)| <b>@deprecated.</b> Please use the 'tickLabelSpacing' property instead. Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--)| <b>@deprecated.</b> Please use the 'isAutoTickLabelSpacing' property instead. Indicates whether the spacing of tick label is automatic |
| [setIsAutoTickLabelSpacing(boolean)](#setIsAutoTickLabelSpacing-boolean-)| <b>@deprecated.</b> Please use the 'isAutoTickLabelSpacing' property instead. Indicates whether the spacing of tick label is automatic |
| [getTickMarkSpacing()](#getTickMarkSpacing--)| <b>@deprecated.</b> Please use the 'tickMarkSpacing' property instead. Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [setTickMarkSpacing(number)](#setTickMarkSpacing-number-)| <b>@deprecated.</b> Please use the 'tickMarkSpacing' property instead. Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [getDisplayUnit()](#getDisplayUnit--)| <b>@deprecated.</b> Please use the 'displayUnit' property instead. Represents the unit label for the specified axis. |
| [setDisplayUnit(DisplayUnitType)](#setDisplayUnit-displayunittype-)| <b>@deprecated.</b> Please use the 'displayUnit' property instead. Represents the unit label for the specified axis. |
| [getCustomUnit()](#getCustomUnit--)| <b>@deprecated.</b> Please use the 'customUnit' property instead. Specifies a custom value for the display unit. |
| [setCustomUnit(number)](#setCustomUnit-number-)| <b>@deprecated.</b> Please use the 'customUnit' property instead. Specifies a custom value for the display unit. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--)| <b>@deprecated.</b> Please use the 'customDisplayUnit' property instead. Specifies a custom value for the display unit. |
| [setCustomDisplayUnit(number)](#setCustomDisplayUnit-number-)| <b>@deprecated.</b> Please use the 'customDisplayUnit' property instead. Specifies a custom value for the display unit. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--)| <b>@deprecated.</b> Please use the 'displayUnitLabel' property instead. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--)| <b>@deprecated.</b> Please use the 'isDisplayUnitLabelShown' property instead. Represents if the display unit label is shown on the specified axis. |
| [setIsDisplayUnitLabelShown(boolean)](#setIsDisplayUnitLabelShown-boolean-)| <b>@deprecated.</b> Please use the 'isDisplayUnitLabelShown' property instead. Represents if the display unit label is shown on the specified axis. |
| [getTitle()](#getTitle--)| <b>@deprecated.</b> Please use the 'title' property instead. Gets the axis' title. |
| [getCategoryType()](#getCategoryType--)| <b>@deprecated.</b> Please use the 'categoryType' property instead. Represents the category axis type. |
| [setCategoryType(CategoryType)](#setCategoryType-categorytype-)| <b>@deprecated.</b> Please use the 'categoryType' property instead. Represents the category axis type. |
| [getBaseUnitScale()](#getBaseUnitScale--)| <b>@deprecated.</b> Please use the 'baseUnitScale' property instead. Represents the base unit scale for the category axis. |
| [setBaseUnitScale(TimeUnit)](#setBaseUnitScale-timeunit-)| <b>@deprecated.</b> Please use the 'baseUnitScale' property instead. Represents the base unit scale for the category axis. |
| [getMajorUnitScale()](#getMajorUnitScale--)| <b>@deprecated.</b> Please use the 'majorUnitScale' property instead. Represents the major unit scale for the category axis. |
| [setMajorUnitScale(TimeUnit)](#setMajorUnitScale-timeunit-)| <b>@deprecated.</b> Please use the 'majorUnitScale' property instead. Represents the major unit scale for the category axis. |
| [getMinorUnitScale()](#getMinorUnitScale--)| <b>@deprecated.</b> Please use the 'minorUnitScale' property instead. Represents the major unit scale for the category axis. |
| [setMinorUnitScale(TimeUnit)](#setMinorUnitScale-timeunit-)| <b>@deprecated.</b> Please use the 'minorUnitScale' property instead. Represents the major unit scale for the category axis. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents if the axis is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents if the axis is visible. |
| [getMajorGridLines()](#getMajorGridLines--)| <b>@deprecated.</b> Please use the 'majorGridLines' property instead. Represents major gridlines on a chart axis. |
| [getMinorGridLines()](#getMinorGridLines--)| <b>@deprecated.</b> Please use the 'minorGridLines' property instead. Represents minor gridlines on a chart axis. |
| [getHasMultiLevelLabels()](#getHasMultiLevelLabels--)| <b>@deprecated.</b> Please use the 'hasMultiLevelLabels' property instead. Indicates whether the labels shall be shown as multi level. |
| [setHasMultiLevelLabels(boolean)](#setHasMultiLevelLabels-boolean-)| <b>@deprecated.</b> Please use the 'hasMultiLevelLabels' property instead. Indicates whether the labels shall be shown as multi level. |
| [getBins()](#getBins--)| <b>@deprecated.</b> Please use the 'bins' property instead. Represents bins on a chart(Histogram/Pareto) axis |
| [getAxisTexts()](#getAxisTexts--)| Gets the labels of the axis after call Chart.Calculate() method. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
minValue : Object;
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
maxValue : Object;
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
Represents the logarithmic base. Default value is 10.Only applies for Excel2007.
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
Readonly. Gets the axis' title.
```javascript
title : Title;
```
### categoryType {#categoryType--}
Represents the category axis type.
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
const { Workbook, ChartType, CategoryType, TimeUnit } = require("aspose.cells.node");
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
const { Workbook, ChartType, CategoryType, TimeUnit } = require("aspose.cells.node");
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
const { Workbook, ChartType } = require("aspose.cells.node");
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
### getArea() {#getArea--}
```javascript
getArea() : Area;
```
**Returns**
[Area](../area/)
### isAutomaticMinValue() {#isAutomaticMinValue--}
```javascript
isAutomaticMinValue() : boolean;
```
### setIsAutomaticMinValue(boolean) {#setIsAutomaticMinValue-boolean-}
```javascript
setIsAutomaticMinValue(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMinValue() {#getMinValue--}
```javascript
getMinValue() : Object;
```
**Remarks**
The minValue type only can be double or DateTime
### setMinValue(Object) {#setMinValue-object-}
```javascript
setMinValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
The minValue type only can be double or DateTime
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```javascript
isAutomaticMaxValue() : boolean;
```
### setIsAutomaticMaxValue(boolean) {#setIsAutomaticMaxValue-boolean-}
```javascript
setIsAutomaticMaxValue(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMaxValue() {#getMaxValue--}
```javascript
getMaxValue() : Object;
```
**Remarks**
The maxValue type only can be double or DateTime
### setMaxValue(Object) {#setMaxValue-object-}
```javascript
setMaxValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
The maxValue type only can be double or DateTime
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```javascript
isAutomaticMajorUnit() : boolean;
```
### setIsAutomaticMajorUnit(boolean) {#setIsAutomaticMajorUnit-boolean-}
```javascript
setIsAutomaticMajorUnit(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMajorUnit() {#getMajorUnit--}
```javascript
getMajorUnit() : number;
```
**Remarks**
The major units must be greater than zero.
### setMajorUnit(number) {#setMajorUnit-number-}
```javascript
setMajorUnit(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The major units must be greater than zero.
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```javascript
isAutomaticMinorUnit() : boolean;
```
### setIsAutomaticMinorUnit(boolean) {#setIsAutomaticMinorUnit-boolean-}
```javascript
setIsAutomaticMinorUnit(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMinorUnit() {#getMinorUnit--}
```javascript
getMinorUnit() : number;
```
**Remarks**
The minor units must be greater than zero.
### setMinorUnit(number) {#setMinorUnit-number-}
```javascript
setMinorUnit(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The minor units must be greater than zero.
### getAxisLine() {#getAxisLine--}
```javascript
getAxisLine() : Line;
```
**Returns**
[Line](../line/)
### getMajorTickMark() {#getMajorTickMark--}
```javascript
getMajorTickMark() : TickMarkType;
```
**Returns**
[TickMarkType](../tickmarktype/)
### setMajorTickMark(TickMarkType) {#setMajorTickMark-tickmarktype-}
```javascript
setMajorTickMark(value: TickMarkType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickMarkType](../tickmarktype/) | The value to set. |
### getMinorTickMark() {#getMinorTickMark--}
```javascript
getMinorTickMark() : TickMarkType;
```
**Returns**
[TickMarkType](../tickmarktype/)
### setMinorTickMark(TickMarkType) {#setMinorTickMark-tickmarktype-}
```javascript
setMinorTickMark(value: TickMarkType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickMarkType](../tickmarktype/) | The value to set. |
### getTickLabelPosition() {#getTickLabelPosition--}
```javascript
getTickLabelPosition() : TickLabelPositionType;
```
**Returns**
[TickLabelPositionType](../ticklabelpositiontype/)
### setTickLabelPosition(TickLabelPositionType) {#setTickLabelPosition-ticklabelpositiontype-}
```javascript
setTickLabelPosition(value: TickLabelPositionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickLabelPositionType](../ticklabelpositiontype/) | The value to set. |
### getCrossAt() {#getCrossAt--}
```javascript
getCrossAt() : number;
```
**Remarks**
The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.
### setCrossAt(number) {#setCrossAt-number-}
```javascript
setCrossAt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.
### getCrossType() {#getCrossType--}
```javascript
getCrossType() : CrossType;
```
**Returns**
[CrossType](../crosstype/)
### setCrossType(CrossType) {#setCrossType-crosstype-}
```javascript
setCrossType(value: CrossType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CrossType](../crosstype/) | The value to set. |
### getLogBase() {#getLogBase--}
```javascript
getLogBase() : number;
```
### setLogBase(number) {#setLogBase-number-}
```javascript
setLogBase(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isLogarithmic() {#isLogarithmic--}
```javascript
isLogarithmic() : boolean;
```
### setIsLogarithmic(boolean) {#setIsLogarithmic-boolean-}
```javascript
setIsLogarithmic(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isPlotOrderReversed() {#isPlotOrderReversed--}
```javascript
isPlotOrderReversed() : boolean;
```
### setIsPlotOrderReversed(boolean) {#setIsPlotOrderReversed-boolean-}
```javascript
setIsPlotOrderReversed(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```javascript
getAxisBetweenCategories() : boolean;
```
**Remarks**
This property applies only to category axes, and it doesn't apply to 3-D charts.
### setAxisBetweenCategories(boolean) {#setAxisBetweenCategories-boolean-}
```javascript
setAxisBetweenCategories(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
This property applies only to category axes, and it doesn't apply to 3-D charts.
### getTickLabels() {#getTickLabels--}
```javascript
getTickLabels() : TickLabels;
```
**Returns**
[TickLabels](../ticklabels/)
### getTickLabelSpacing() {#getTickLabelSpacing--}
```javascript
getTickLabelSpacing() : number;
```
**Remarks**
The number must be between 1 and 31999.
### setTickLabelSpacing(number) {#setTickLabelSpacing-number-}
```javascript
setTickLabelSpacing(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The number must be between 1 and 31999.
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```javascript
isAutoTickLabelSpacing() : boolean;
```
### setIsAutoTickLabelSpacing(boolean) {#setIsAutoTickLabelSpacing-boolean-}
```javascript
setIsAutoTickLabelSpacing(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTickMarkSpacing() {#getTickMarkSpacing--}
```javascript
getTickMarkSpacing() : number;
```
**Remarks**
The number must be between 1 and 31999.
### setTickMarkSpacing(number) {#setTickMarkSpacing-number-}
```javascript
setTickMarkSpacing(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The number must be between 1 and 31999.
### getDisplayUnit() {#getDisplayUnit--}
```javascript
getDisplayUnit() : DisplayUnitType;
```
**Returns**
[DisplayUnitType](../displayunittype/)
### setDisplayUnit(DisplayUnitType) {#setDisplayUnit-displayunittype-}
```javascript
setDisplayUnit(value: DisplayUnitType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DisplayUnitType](../displayunittype/) | The value to set. |
### getCustomUnit() {#getCustomUnit--}
```javascript
getCustomUnit() : number;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use Axis.CustomDisplayUnit property. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### setCustomUnit(number) {#setCustomUnit-number-}
```javascript
setCustomUnit(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use Axis.CustomDisplayUnit property. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```javascript
getCustomDisplayUnit() : number;
```
### setCustomDisplayUnit(number) {#setCustomDisplayUnit-number-}
```javascript
setCustomDisplayUnit(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```javascript
getDisplayUnitLabel() : DisplayUnitLabel;
```
**Returns**
[DisplayUnitLabel](../displayunitlabel/)
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```javascript
isDisplayUnitLabelShown() : boolean;
```
**Remarks**
The default value is True.
### setIsDisplayUnitLabelShown(boolean) {#setIsDisplayUnitLabelShown-boolean-}
```javascript
setIsDisplayUnitLabelShown(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is True.
### getTitle() {#getTitle--}
```javascript
getTitle() : Title;
```
**Returns**
[Title](../title/)
### getCategoryType() {#getCategoryType--}
```javascript
getCategoryType() : CategoryType;
```
**Returns**
[CategoryType](../categorytype/)
### setCategoryType(CategoryType) {#setCategoryType-categorytype-}
```javascript
setCategoryType(value: CategoryType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CategoryType](../categorytype/) | The value to set. |
### getBaseUnitScale() {#getBaseUnitScale--}
```javascript
getBaseUnitScale() : TimeUnit;
```
**Returns**
[TimeUnit](../timeunit/)
**Remarks**
Setting this property only takes effect when the CategoryType property is set to TimeScale.
### setBaseUnitScale(TimeUnit) {#setBaseUnitScale-timeunit-}
```javascript
setBaseUnitScale(value: TimeUnit) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |
**Remarks**
Setting this property only takes effect when the CategoryType property is set to TimeScale.
### getMajorUnitScale() {#getMajorUnitScale--}
```javascript
getMajorUnitScale() : TimeUnit;
```
**Returns**
[TimeUnit](../timeunit/)
### setMajorUnitScale(TimeUnit) {#setMajorUnitScale-timeunit-}
```javascript
setMajorUnitScale(value: TimeUnit) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |
### getMinorUnitScale() {#getMinorUnitScale--}
```javascript
getMinorUnitScale() : TimeUnit;
```
**Returns**
[TimeUnit](../timeunit/)
### setMinorUnitScale(TimeUnit) {#setMinorUnitScale-timeunit-}
```javascript
setMinorUnitScale(value: TimeUnit) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |
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
### getMajorGridLines() {#getMajorGridLines--}
```javascript
getMajorGridLines() : Line;
```
**Returns**
[Line](../line/)
### getMinorGridLines() {#getMinorGridLines--}
```javascript
getMinorGridLines() : Line;
```
**Returns**
[Line](../line/)
### getHasMultiLevelLabels() {#getHasMultiLevelLabels--}
```javascript
getHasMultiLevelLabels() : boolean;
```
**Remarks**
Only valid for category axis.
### setHasMultiLevelLabels(boolean) {#setHasMultiLevelLabels-boolean-}
```javascript
setHasMultiLevelLabels(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only valid for category axis.
### getBins() {#getBins--}
```javascript
getBins() : AxisBins;
```
**Returns**
[AxisBins](../axisbins/)
### getAxisTexts() {#getAxisTexts--}
Gets the labels of the axis after call Chart.Calculate() method.
```javascript
getAxisTexts() : string[];
```
**Returns**
string[]
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
