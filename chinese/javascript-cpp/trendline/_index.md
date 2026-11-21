---
title: Trendline
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a trendline in a chart.
type: docs
url: /zh/javascript-cpp/trendline/
---

## Trendline class

Represents a trendline in a chart.

```javascript
class Trendline extends Line;
```


### Example
```javascript
const { Workbook, ChartType, TrendlineType, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
//向 Excel 对象添加新工作表
var sheetIndex = workbook.worksheets.add();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向 "A4" 单元格添加示例值
worksheet.cells.get("A4").putValue(200);
//向 "B1" 单元格添加示例值
worksheet.cells.get("B1").putValue(60);
//向 "B2" 单元格添加示例值
worksheet.cells.get("B2").putValue(32);
//向 "B3" 单元格添加示例值
worksheet.cells.get("B3").putValue(50);
//向 "B4" 单元格添加示例值
worksheet.cells.get("B4").putValue(40);
//向 "C1" 单元格添加示例值作为类别数据
worksheet.cells.get("C1").putValue("Q1");
//向 "C2" 单元格添加示例值作为类别数据
worksheet.cells.get("C2").putValue("Q2");
//将示例值添加到 "C3" 单元格作为类别数据
worksheet.cells.get("C3").putValue("Y1");
//将示例值添加到 "C4" 单元格作为类别数据
worksheet.cells.get("C4").putValue("Y2");
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//向图表添加 NSeries（图表数据源），范围从 "A1" 单元格到 "B4"
chart.nSeries.add("A1:B4", true);
//设置 NSeries 类别数据的数据源
chart.nSeries.categoryData = "C1:C4";
//添加线性趋势线
var index = chart.nSeries.get(0).trendLines.add(TrendlineType.Linear);
var trendline = chart.nSeries.get(0).trendLines.get(index);
//设置趋势线的自定义名称。
trendline.name = "Linear";
//在图表上显示方程式
trendline.displayEquation = true;
//在图表上显示 R 平方值
trendline.displayRSquared = true;
//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Constructors

| Name | Description |
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



