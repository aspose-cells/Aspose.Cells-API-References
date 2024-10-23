---
title: Trendline
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a trendline in a chart.
type: docs
url: /nodejs-cpp/trendline/
---

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
var sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.getCells().get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.getCells().get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.getCells().get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.getCells().get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.getCells().get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.getCells().get("C4").putValue("Y2");
//Adding a chart to the worksheet
var chartIndex = worksheet.getCharts().add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.getNSeries().add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.getNSeries().setCategoryData("C1:C4");
//adding a linear trendline
var index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.Linear);
var trendline = chart.getNSeries().get(0).getTrendLines().get(index);
//Setting the custom name of the trendline.
trendline.setName("Linear");
//Displaying the equation on chart
trendline.setDisplayEquation(true);
//Displaying the R-Squared value on chart
trendline.setDisplayRSquared(true);
//Saving the Excel file
workbook.save("output/ChartsTrendline.xls");
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(Line)](#constructor-line-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [isNameAuto()](#isNameAuto--)| Returns if Microsoft Excel automatically determines the name of the trendline. |
| [setIsNameAuto(boolean)](#setIsNameAuto-boolean-)| Returns if Microsoft Excel automatically determines the name of the trendline. |
| [getType()](#getType--)| Returns the trendline type. |
| [getName()](#getName--)| Returns the name of the trendline. |
| [setName(string)](#setName-string-)| Returns the name of the trendline. |
| [getOrder()](#getOrder--)| Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [setOrder(number)](#setOrder-number-)| Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [getPeriod()](#getPeriod--)| Returns or sets the period for the moving-average trendline. |
| [setPeriod(number)](#setPeriod-number-)| Returns or sets the period for the moving-average trendline. |
| [getForward()](#getForward--)| Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [setForward(number)](#setForward-number-)| Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [getBackward()](#getBackward--)| Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [setBackward(number)](#setBackward-number-)| Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [getDisplayEquation()](#getDisplayEquation--)| Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [setDisplayEquation(boolean)](#setDisplayEquation-boolean-)| Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [getDisplayRSquared()](#getDisplayRSquared--)| Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [setDisplayRSquared(boolean)](#setDisplayRSquared-boolean-)| Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [getIntercept()](#getIntercept--)| Returns or sets the point where the trendline crosses the value axis. |
| [setIntercept(number)](#setIntercept-number-)| Returns or sets the point where the trendline crosses the value axis. |
| [getDataLabels()](#getDataLabels--)| Represents the DataLabels object for the specified series. |
| [getLegendEntry()](#getLegendEntry--)| Gets the legend entry according to this trendline |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCompoundType()](#getCompoundType--)| Specifies the compound line type |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| Specifies the compound line type |
| [getDashType()](#getDashType--)| Specifies the dash line type |
| [setDashType(MsoLineDashStyle)](#setDashType-msolinedashstyle-)| Specifies the dash line type |
| [getCapType()](#getCapType--)| Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| Specifies the joining caps. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| Specifies the joining caps. |
| [getBeginType()](#getBeginType--)| Specifies an arrowhead for the begin of a line. |
| [setBeginType(MsoArrowheadStyle)](#setBeginType-msoarrowheadstyle-)| Specifies an arrowhead for the begin of a line. |
| [getEndType()](#getEndType--)| Specifies an arrowhead for the end of a line. |
| [setEndType(MsoArrowheadStyle)](#setEndType-msoarrowheadstyle-)| Specifies an arrowhead for the end of a line. |
| [getBeginArrowLength()](#getBeginArrowLength--)| Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowLength(MsoArrowheadLength)](#setBeginArrowLength-msoarrowheadlength-)| Specifies the length of the arrowhead for the begin of a line. |
| [getEndArrowLength()](#getEndArrowLength--)| Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowLength(MsoArrowheadLength)](#setEndArrowLength-msoarrowheadlength-)| Specifies the length of the arrowhead for the end of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--)| Specifies the width of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(MsoArrowheadWidth)](#setBeginArrowWidth-msoarrowheadwidth-)| Specifies the width of the arrowhead for the begin of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--)| Specifies the width of the arrowhead for the end of a line. |
| [setEndArrowWidth(MsoArrowheadWidth)](#setEndArrowWidth-msoarrowheadwidth-)| Specifies the width of the arrowhead for the end of a line. |
| [getThemeColor()](#getThemeColor--)| Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets and sets the theme color. |
| [getColor()](#getColor--)| Represents the [Color](../color/) of the line. |
| [setColor(Color)](#setColor-color-)| Represents the [Color](../color/) of the line. |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getStyle()](#getStyle--)| Represents the style of the line. |
| [setStyle(LineType)](#setStyle-linetype-)| Represents the style of the line. |
| [getWeight()](#getWeight--)| Gets or sets the [WeightType](../weighttype/) of the line. |
| [setWeight(WeightType)](#setWeight-weighttype-)| Gets or sets the [WeightType](../weighttype/) of the line. |
| [getWeightPt()](#getWeightPt--)| Gets or sets the weight of the line in unit of points. |
| [setWeightPt(number)](#setWeightPt-number-)| Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--)| Gets or sets the weight of the line in unit of pixels. |
| [setWeightPx(number)](#setWeightPx-number-)| Gets or sets the weight of the line in unit of pixels. |
| [getFormattingType()](#getFormattingType--)| Gets or sets format type. |
| [setFormattingType(ChartLineFormattingType)](#setFormattingType-chartlineformattingtype-)| Gets or sets format type. |
| [isAutomaticColor()](#isAutomaticColor--)| Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--)| Represents whether the line is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Represents whether the line is visible. |
| [isAuto()](#isAuto--)| Indicates whether this line style is auto assigned. |
| [setIsAuto(boolean)](#setIsAuto-boolean-)| Indicates whether this line style is auto assigned. |
| [getGradientFill()](#getGradientFill--)| Represents gradient fill. |


### constructor(Line) {#constructor-line-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Line);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Line | The parent object. |

### isNameAuto() {#isNameAuto--}

Returns if Microsoft Excel automatically determines the name of the trendline.

```javascript
isNameAuto() : boolean;
```


### setIsNameAuto(boolean) {#setIsNameAuto-boolean-}

Returns if Microsoft Excel automatically determines the name of the trendline.

```javascript
setIsNameAuto(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getType() {#getType--}

Returns the trendline type.

```javascript
getType() : TrendlineType;
```


**Returns**

[TrendlineType](../trendlinetype/)

### getName() {#getName--}

Returns the name of the trendline.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Returns the name of the trendline.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getOrder() {#getOrder--}

Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.

```javascript
getOrder() : number;
```


### setOrder(number) {#setOrder-number-}

Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.

```javascript
setOrder(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPeriod() {#getPeriod--}

Returns or sets the period for the moving-average trendline.

```javascript
getPeriod() : number;
```


**Remarks**

This value should be between 2 and 255. And it must be less than the number of the chart points in the series

### setPeriod(number) {#setPeriod-number-}

Returns or sets the period for the moving-average trendline.

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

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.

```javascript
getForward() : number;
```


### setForward(number) {#setForward-number-}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.

```javascript
setForward(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBackward() {#getBackward--}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

```javascript
getBackward() : number;
```


### setBackward(number) {#setBackward-number-}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

```javascript
setBackward(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getDisplayEquation() {#getDisplayEquation--}

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

```javascript
getDisplayEquation() : boolean;
```


### setDisplayEquation(boolean) {#setDisplayEquation-boolean-}

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

```javascript
setDisplayEquation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayRSquared() {#getDisplayRSquared--}

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

```javascript
getDisplayRSquared() : boolean;
```


### setDisplayRSquared(boolean) {#setDisplayRSquared-boolean-}

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

```javascript
setDisplayRSquared(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIntercept() {#getIntercept--}

Returns or sets the point where the trendline crosses the value axis.

```javascript
getIntercept() : number;
```


### setIntercept(number) {#setIntercept-number-}

Returns or sets the point where the trendline crosses the value axis.

```javascript
setIntercept(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getDataLabels() {#getDataLabels--}

Represents the DataLabels object for the specified series.

```javascript
getDataLabels() : DataLabels;
```


**Returns**

[DataLabels](../datalabels/)

### getLegendEntry() {#getLegendEntry--}

Gets the legend entry according to this trendline

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

Specifies the compound line type

```javascript
getCompoundType() : MsoLineStyle;
```


**Returns**

[MsoLineStyle](../msolinestyle/)

### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}

Specifies the compound line type

```javascript
setCompoundType(value: MsoLineStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |

### getDashType() {#getDashType--}

Specifies the dash line type

```javascript
getDashType() : MsoLineDashStyle;
```


**Returns**

[MsoLineDashStyle](../msolinedashstyle/)

### setDashType(MsoLineDashStyle) {#setDashType-msolinedashstyle-}

Specifies the dash line type

```javascript
setDashType(value: MsoLineDashStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |

### getCapType() {#getCapType--}

Specifies the ending caps.

```javascript
getCapType() : LineCapType;
```


**Returns**

[LineCapType](../linecaptype/)

### setCapType(LineCapType) {#setCapType-linecaptype-}

Specifies the ending caps.

```javascript
setCapType(value: LineCapType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |

### getJoinType() {#getJoinType--}

Specifies the joining caps.

```javascript
getJoinType() : LineJoinType;
```


**Returns**

[LineJoinType](../linejointype/)

### setJoinType(LineJoinType) {#setJoinType-linejointype-}

Specifies the joining caps.

```javascript
setJoinType(value: LineJoinType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |

### getBeginType() {#getBeginType--}

Specifies an arrowhead for the begin of a line.

```javascript
getBeginType() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setBeginType(MsoArrowheadStyle) {#setBeginType-msoarrowheadstyle-}

Specifies an arrowhead for the begin of a line.

```javascript
setBeginType(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getEndType() {#getEndType--}

Specifies an arrowhead for the end of a line.

```javascript
getEndType() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setEndType(MsoArrowheadStyle) {#setEndType-msoarrowheadstyle-}

Specifies an arrowhead for the end of a line.

```javascript
setEndType(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getBeginArrowLength() {#getBeginArrowLength--}

Specifies the length of the arrowhead for the begin of a line.

```javascript
getBeginArrowLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setBeginArrowLength(MsoArrowheadLength) {#setBeginArrowLength-msoarrowheadlength-}

Specifies the length of the arrowhead for the begin of a line.

```javascript
setBeginArrowLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getEndArrowLength() {#getEndArrowLength--}

Specifies the length of the arrowhead for the end of a line.

```javascript
getEndArrowLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setEndArrowLength(MsoArrowheadLength) {#setEndArrowLength-msoarrowheadlength-}

Specifies the length of the arrowhead for the end of a line.

```javascript
setEndArrowLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getBeginArrowWidth() {#getBeginArrowWidth--}

Specifies the width of the arrowhead for the begin of a line.

```javascript
getBeginArrowWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setBeginArrowWidth(MsoArrowheadWidth) {#setBeginArrowWidth-msoarrowheadwidth-}

Specifies the width of the arrowhead for the begin of a line.

```javascript
setBeginArrowWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getEndArrowWidth() {#getEndArrowWidth--}

Specifies the width of the arrowhead for the end of a line.

```javascript
getEndArrowWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setEndArrowWidth(MsoArrowheadWidth) {#setEndArrowWidth-msoarrowheadwidth-}

Specifies the width of the arrowhead for the end of a line.

```javascript
setEndArrowWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getThemeColor() {#getThemeColor--}

Gets and sets the theme color.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

**Remarks**

If the foreground color is not a theme color, NULL will be returned.

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets and sets the theme color.

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

Represents the [Color](../color/) of the line.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Represents the [Color](../color/) of the line.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStyle() {#getStyle--}

Represents the style of the line.

```javascript
getStyle() : LineType;
```


**Returns**

[LineType](../linetype/)

### setStyle(LineType) {#setStyle-linetype-}

Represents the style of the line.

```javascript
setStyle(value: LineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineType](../linetype/) | The value to set. |

### getWeight() {#getWeight--}

Gets or sets the [WeightType](../weighttype/) of the line.

```javascript
getWeight() : WeightType;
```


**Returns**

[WeightType](../weighttype/)

### setWeight(WeightType) {#setWeight-weighttype-}

Gets or sets the [WeightType](../weighttype/) of the line.

```javascript
setWeight(value: WeightType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WeightType](../weighttype/) | The value to set. |

### getWeightPt() {#getWeightPt--}

Gets or sets the weight of the line in unit of points.

```javascript
getWeightPt() : number;
```


### setWeightPt(number) {#setWeightPt-number-}

Gets or sets the weight of the line in unit of points.

```javascript
setWeightPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWeightPx() {#getWeightPx--}

Gets or sets the weight of the line in unit of pixels.

```javascript
getWeightPx() : number;
```


### setWeightPx(number) {#setWeightPx-number-}

Gets or sets the weight of the line in unit of pixels.

```javascript
setWeightPx(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFormattingType() {#getFormattingType--}

Gets or sets format type.

```javascript
getFormattingType() : ChartLineFormattingType;
```


**Returns**

[ChartLineFormattingType](../chartlineformattingtype/)

### setFormattingType(ChartLineFormattingType) {#setFormattingType-chartlineformattingtype-}

Gets or sets format type.

```javascript
setFormattingType(value: ChartLineFormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartLineFormattingType](../chartlineformattingtype/) | The value to set. |

### isAutomaticColor() {#isAutomaticColor--}

Indicates whether the color of line is automatic assigned.

```javascript
isAutomaticColor() : boolean;
```


### isVisible() {#isVisible--}

Represents whether the line is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Represents whether the line is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAuto() {#isAuto--}

Indicates whether this line style is auto assigned.

```javascript
isAuto() : boolean;
```


### setIsAuto(boolean) {#setIsAuto-boolean-}

Indicates whether this line style is auto assigned.

```javascript
setIsAuto(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getGradientFill() {#getGradientFill--}

Represents gradient fill.

```javascript
getGradientFill() : GradientFill;
```


**Returns**

[GradientFill](../gradientfill/)


