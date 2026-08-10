---
title: "Trendline"
linktitle: "Trendline"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a trendline in a chart."
type: docs
weight: 4360
url: /nodejs/aspose.cells/trendline/
---

## Trendline class

Represents a trendline in a chart.

## Methods

| Name | Description |
| --- | --- |
| [getBackward()](#getbackward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of p |
| [getBeginArrowLength()](#getbeginarrowlength) | Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer c |
| [getBeginArrowWidth()](#getbeginarrowwidth) | Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer con |
| [getBeginType()](#getbegintype) | Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [getCapType()](#getcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [getColor()](#getcolor) | Represents the com.aspose.cells.Color of the line. |
| [getCompoundType()](#getcompoundtype) | Specifies the compound line type The value of the property is MsoLineStyle integer constant. |
| [getDashType()](#getdashtype) | Specifies the dash line type The value of the property is MsoLineDashStyle integer constant. |
| [getDataLabels()](#getdatalabels) | Represents the DataLabels object for the specified series. |
| [getDisplayEquation()](#getdisplayequation) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value).  |
| [getDisplayRSquared()](#getdisplayrsquared) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). S |
| [getEndArrowLength()](#getendarrowlength) | Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer con |
| [getEndArrowWidth()](#getendarrowwidth) | Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer const |
| [getEndType()](#getendtype) | Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [getFormattingType()](#getformattingtype) | Gets or sets format type. The value of the property is ChartLineFormattingType integer constant. |
| [getForward()](#getforward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of pe |
| [getGradientFill()](#getgradientfill) | Represents gradient fill. |
| [getIntercept()](#getintercept) | Returns or sets the point where the trendline crosses the value axis. |
| [getJoinType()](#getjointype) | Specifies the joining caps. The value of the property is LineJoinType integer constant. |
| [getLegendEntry()](#getlegendentry) | Gets the legend entry according to this trendline |
| [getName()](#getname) | Returns the name of the trendline. |
| [getOrder()](#getorder) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be |
| [getPeriod()](#getperiod) | Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less |
| [getStyle()](#getstyle) | Represents the style of the line. The value of the property is LineType integer constant. |
| [getThemeColor()](#getthemecolor) | Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned. |
| [getTransparency()](#gettransparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#gettype) | Returns the trendline type. The value of the property is TrendlineType integer constant. |
| [getWeight()](#getweight) | Gets or sets the WeightType of the line. The value of the property is WeightType integer constant. |
| [getWeightPt()](#getweightpt) | Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getweightpx) | Gets or sets the weight of the line in unit of pixels. |
| [isAuto()](#isauto) | Indicates whether this line style is auto assigned. |
| [isAutomaticColor()](#isautomaticcolor) | Indicates whether the color of line is automatic assigned. |
| [isInterceptAuto()](#isinterceptauto) | Indicates whether Microsoft Workbook automatically determines the intercept of the trendline. |
| [isNameAuto()](#isnameauto) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [isVisible()](#isvisible) | Represents whether the line is visible. |
| [setAuto()](#setauto) | Indicates whether this line style is auto assigned. |
| [setBackward()](#setbackward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of p |
| [setBeginArrowLength()](#setbeginarrowlength) | Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer c |
| [setBeginArrowWidth()](#setbeginarrowwidth) | Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer con |
| [setBeginType()](#setbegintype) | Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [setCapType()](#setcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [setColor()](#setcolor) | Represents the com.aspose.cells.Color of the line. |
| [setCompoundType()](#setcompoundtype) | Specifies the compound line type The value of the property is MsoLineStyle integer constant. |
| [setDashType()](#setdashtype) | Specifies the dash line type The value of the property is MsoLineDashStyle integer constant. |
| [setDisplayEquation()](#setdisplayequation) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value).  |
| [setDisplayRSquared()](#setdisplayrsquared) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). S |
| [setEndArrowLength()](#setendarrowlength) | Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer con |
| [setEndArrowWidth()](#setendarrowwidth) | Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer const |
| [setEndType()](#setendtype) | Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [setFormattingType()](#setformattingtype) | Gets or sets format type. The value of the property is ChartLineFormattingType integer constant. |
| [setForward()](#setforward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of pe |
| [setIntercept()](#setintercept) | Returns or sets the point where the trendline crosses the value axis. |
| [setInterceptAuto()](#setinterceptauto) | Sets whether Microsoft Workbook automatically determines the intercept of the trendline. |
| [setJoinType()](#setjointype) | Specifies the joining caps. The value of the property is LineJoinType integer constant. |
| [setName()](#setname) | Returns the name of the trendline. |
| [setNameAuto()](#setnameauto) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [setOrder()](#setorder) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be |
| [setPeriod()](#setperiod) | Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less |
| [setStyle()](#setstyle) | Represents the style of the line. The value of the property is LineType integer constant. |
| [setThemeColor()](#setthemecolor) | Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned. |
| [setTransparency()](#settransparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setVisible()](#setvisible) | Represents whether the line is visible. |
| [setWeight()](#setweight) | Gets or sets the WeightType of the line. The value of the property is WeightType integer constant. |
| [setWeightPt()](#setweightpt) | Gets or sets the weight of the line in unit of points. |
| [setWeightPx()](#setweightpx) | Gets or sets the weight of the line in unit of pixels. |

### getBackward() {#getbackward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

### getBeginArrowLength() {#getbeginarrowlength}

Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer constant.

### getBeginArrowWidth() {#getbeginarrowwidth}

Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer constant.

### getBeginType() {#getbegintype}

Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant.

### getCapType() {#getcaptype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

### getColor() {#getcolor}

Represents the com.aspose.cells.Color of the line.

### getCompoundType() {#getcompoundtype}

Specifies the compound line type The value of the property is MsoLineStyle integer constant.

### getDashType() {#getdashtype}

Specifies the dash line type The value of the property is MsoLineDashStyle integer constant.

### getDataLabels() {#getdatalabels}

Represents the DataLabels object for the specified series.

### getDisplayEquation() {#getdisplayequation}

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

### getDisplayRSquared() {#getdisplayrsquared}

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

### getEndArrowLength() {#getendarrowlength}

Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer constant.

### getEndArrowWidth() {#getendarrowwidth}

Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer constant.

### getEndType() {#getendtype}

Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant.

### getFormattingType() {#getformattingtype}

Gets or sets format type. The value of the property is ChartLineFormattingType integer constant.

### getForward() {#getforward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.

### getGradientFill() {#getgradientfill}

Represents gradient fill.

### getIntercept() {#getintercept}

Returns or sets the point where the trendline crosses the value axis.

### getJoinType() {#getjointype}

Specifies the joining caps. The value of the property is LineJoinType integer constant.

### getLegendEntry() {#getlegendentry}

Gets the legend entry according to this trendline

### getName() {#getname}

Returns the name of the trendline.

### getOrder() {#getorder}

Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.

### getPeriod() {#getperiod}

Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less than the number of the chart points in the series

### getStyle() {#getstyle}

Represents the style of the line. The value of the property is LineType integer constant.

### getThemeColor() {#getthemecolor}

Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

### getTransparency() {#gettransparency}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

### getType() {#gettype}

Returns the trendline type. The value of the property is TrendlineType integer constant.

### getWeight() {#getweight}

Gets or sets the WeightType of the line. The value of the property is WeightType integer constant.

### getWeightPt() {#getweightpt}

Gets or sets the weight of the line in unit of points.

### getWeightPx() {#getweightpx}

Gets or sets the weight of the line in unit of pixels.

### isAuto() {#isauto}

Indicates whether this line style is auto assigned.

### isAutomaticColor() {#isautomaticcolor}

Indicates whether the color of line is automatic assigned.

### isInterceptAuto() {#isinterceptauto}

Indicates whether Microsoft Workbook automatically determines the intercept of the trendline.

### isNameAuto() {#isnameauto}

Returns if Microsoft Excel automatically determines the name of the trendline.

### isVisible() {#isvisible}

Represents whether the line is visible.

### setAuto() {#setauto}

Indicates whether this line style is auto assigned.

### setBackward() {#setbackward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

### setBeginArrowLength() {#setbeginarrowlength}

Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer constant.

### setBeginArrowWidth() {#setbeginarrowwidth}

Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer constant.

### setBeginType() {#setbegintype}

Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant.

### setCapType() {#setcaptype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

### setColor() {#setcolor}

Represents the com.aspose.cells.Color of the line.

### setCompoundType() {#setcompoundtype}

Specifies the compound line type The value of the property is MsoLineStyle integer constant.

### setDashType() {#setdashtype}

Specifies the dash line type The value of the property is MsoLineDashStyle integer constant.

### setDisplayEquation() {#setdisplayequation}

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

### setDisplayRSquared() {#setdisplayrsquared}

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

### setEndArrowLength() {#setendarrowlength}

Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer constant.

### setEndArrowWidth() {#setendarrowwidth}

Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer constant.

### setEndType() {#setendtype}

Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant.

### setFormattingType() {#setformattingtype}

Gets or sets format type. The value of the property is ChartLineFormattingType integer constant.

### setForward() {#setforward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.

### setIntercept() {#setintercept}

Returns or sets the point where the trendline crosses the value axis.

### setInterceptAuto() {#setinterceptauto}

Sets whether Microsoft Workbook automatically determines the intercept of the trendline.

### setJoinType() {#setjointype}

Specifies the joining caps. The value of the property is LineJoinType integer constant.

### setName() {#setname}

Returns the name of the trendline.

### setNameAuto() {#setnameauto}

Returns if Microsoft Excel automatically determines the name of the trendline.

### setOrder() {#setorder}

Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.

### setPeriod() {#setperiod}

Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less than the number of the chart points in the series

### setStyle() {#setstyle}

Represents the style of the line. The value of the property is LineType integer constant.

### setThemeColor() {#setthemecolor}

Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

### setTransparency() {#settransparency}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

### setVisible() {#setvisible}

Represents whether the line is visible.

### setWeight() {#setweight}

Gets or sets the WeightType of the line. The value of the property is WeightType integer constant.

### setWeightPt() {#setweightpt}

Gets or sets the weight of the line in unit of points.

### setWeightPx() {#setweightpx}

Gets or sets the weight of the line in unit of pixels.
