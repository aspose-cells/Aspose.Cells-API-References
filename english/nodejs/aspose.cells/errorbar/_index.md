---
title: "ErrorBar"
linktitle: "ErrorBar"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents error bar of data series."
type: docs
weight: 1330
url: /nodejs/aspose.cells/errorbar/
---

## ErrorBar class

Represents error bar of data series.

## Methods

| Name | Description |
| --- | --- |
| [getAmount()](#getamount) | Represents amount of error bar. The amount must be greater than or equal to zero. |
| [getBeginArrowLength()](#getbeginarrowlength) | Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer c |
| [getBeginArrowWidth()](#getbeginarrowwidth) | Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer con |
| [getBeginType()](#getbegintype) | Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [getCapType()](#getcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [getColor()](#getcolor) | Represents the com.aspose.cells.Color of the line. |
| [getCompoundType()](#getcompoundtype) | Specifies the compound line type The value of the property is MsoLineStyle integer constant. |
| [getDashType()](#getdashtype) | Specifies the dash line type The value of the property is MsoLineDashStyle integer constant. |
| [getDisplayType()](#getdisplaytype) | Represents the display type of error bar. The value of the property is ErrorBarDisplayType integer constant. |
| [getEndArrowLength()](#getendarrowlength) | Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer con |
| [getEndArrowWidth()](#getendarrowwidth) | Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer const |
| [getEndType()](#getendtype) | Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [getFormattingType()](#getformattingtype) | Gets or sets format type. The value of the property is ChartLineFormattingType integer constant. |
| [getGradientFill()](#getgradientfill) | Represents gradient fill. |
| [getJoinType()](#getjointype) | Specifies the joining caps. The value of the property is LineJoinType integer constant. |
| [getMinusValue()](#getminusvalue) | Represents negative error amount when error bar type is Custom. |
| [getPlusValue()](#getplusvalue) | Represents positive error amount when error bar type is Custom. |
| [getShowMarkerTTop()](#getshowmarkerttop) | Indicates if formatting error bars with a T-top. |
| [getStyle()](#getstyle) | Represents the style of the line. The value of the property is LineType integer constant. |
| [getThemeColor()](#getthemecolor) | Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned. |
| [getTransparency()](#gettransparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#gettype) | Represents error bar amount type. The value of the property is ErrorBarType integer constant. |
| [getWeight()](#getweight) | Gets or sets the WeightType of the line. The value of the property is WeightType integer constant. |
| [getWeightPt()](#getweightpt) | Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getweightpx) | Gets or sets the weight of the line in unit of pixels. |
| [isAuto()](#isauto) | Indicates whether this line style is auto assigned. |
| [isAutomaticColor()](#isautomaticcolor) | Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isvisible) | Represents whether the line is visible. |
| [setAmount()](#setamount) | Represents amount of error bar. The amount must be greater than or equal to zero. |
| [setAuto()](#setauto) | Indicates whether this line style is auto assigned. |
| [setBeginArrowLength()](#setbeginarrowlength) | Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer c |
| [setBeginArrowWidth()](#setbeginarrowwidth) | Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer con |
| [setBeginType()](#setbegintype) | Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [setCapType()](#setcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [setColor()](#setcolor) | Represents the com.aspose.cells.Color of the line. |
| [setCompoundType()](#setcompoundtype) | Specifies the compound line type The value of the property is MsoLineStyle integer constant. |
| [setDashType()](#setdashtype) | Specifies the dash line type The value of the property is MsoLineDashStyle integer constant. |
| [setDisplayType()](#setdisplaytype) | Represents the display type of error bar. The value of the property is ErrorBarDisplayType integer constant. |
| [setEndArrowLength()](#setendarrowlength) | Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer con |
| [setEndArrowWidth()](#setendarrowwidth) | Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer const |
| [setEndType()](#setendtype) | Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [setFormattingType()](#setformattingtype) | Gets or sets format type. The value of the property is ChartLineFormattingType integer constant. |
| [setJoinType()](#setjointype) | Specifies the joining caps. The value of the property is LineJoinType integer constant. |
| [setMinusValue()](#setminusvalue) | Represents negative error amount when error bar type is Custom. |
| [setPlusValue()](#setplusvalue) | Represents positive error amount when error bar type is Custom. |
| [setShowMarkerTTop()](#setshowmarkerttop) | Indicates if formatting error bars with a T-top. |
| [setStyle()](#setstyle) | Represents the style of the line. The value of the property is LineType integer constant. |
| [setThemeColor()](#setthemecolor) | Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned. |
| [setTransparency()](#settransparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setType()](#settype) | Represents error bar amount type. The value of the property is ErrorBarType integer constant. |
| [setVisible()](#setvisible) | Represents whether the line is visible. |
| [setWeight()](#setweight) | Gets or sets the WeightType of the line. The value of the property is WeightType integer constant. |
| [setWeightPt()](#setweightpt) | Gets or sets the weight of the line in unit of points. |
| [setWeightPx()](#setweightpx) | Gets or sets the weight of the line in unit of pixels. |

### getAmount() {#getamount}

Represents amount of error bar. The amount must be greater than or equal to zero.

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

### getDisplayType() {#getdisplaytype}

Represents the display type of error bar. The value of the property is ErrorBarDisplayType integer constant.

### getEndArrowLength() {#getendarrowlength}

Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer constant.

### getEndArrowWidth() {#getendarrowwidth}

Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer constant.

### getEndType() {#getendtype}

Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant.

### getFormattingType() {#getformattingtype}

Gets or sets format type. The value of the property is ChartLineFormattingType integer constant.

### getGradientFill() {#getgradientfill}

Represents gradient fill.

### getJoinType() {#getjointype}

Specifies the joining caps. The value of the property is LineJoinType integer constant.

### getMinusValue() {#getminusvalue}

Represents negative error amount when error bar type is Custom.

### getPlusValue() {#getplusvalue}

Represents positive error amount when error bar type is Custom.

### getShowMarkerTTop() {#getshowmarkerttop}

Indicates if formatting error bars with a T-top.

### getStyle() {#getstyle}

Represents the style of the line. The value of the property is LineType integer constant.

### getThemeColor() {#getthemecolor}

Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

### getTransparency() {#gettransparency}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

### getType() {#gettype}

Represents error bar amount type. The value of the property is ErrorBarType integer constant.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
cells.get("C1").putValue("Q1");
cells.get("C2").putValue("Q2");
cells.get("C3").putValue("Y1");
cells.get("C4").putValue("Y2");
var chartIndex = workbook.getWorksheets().get(0).getCharts().add(aspose.cells.ChartType.COLUMN, 11, 0, 27, 10);
var chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:B4", true);
chart.getNSeries().setCategoryData("C1:C4");
for (var i = 0; i < chart.getNSeries().getCount(); i++)
{
var aseries = chart.getNSeries().get(i);
//Sets custom error bar type
aseries.getXErrorBar().setType(aspose.cells.ErrorBarType.CUSTOM);
aseries.getXErrorBar().setPlusValue("=Sheet1!A1");
aseries.getXErrorBar().setMinusValue("=Sheet1!A2");
}
```

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

### isVisible() {#isvisible}

Represents whether the line is visible.

### setAmount() {#setamount}

Represents amount of error bar. The amount must be greater than or equal to zero.

### setAuto() {#setauto}

Indicates whether this line style is auto assigned.

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

### setDisplayType() {#setdisplaytype}

Represents the display type of error bar. The value of the property is ErrorBarDisplayType integer constant.

### setEndArrowLength() {#setendarrowlength}

Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer constant.

### setEndArrowWidth() {#setendarrowwidth}

Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer constant.

### setEndType() {#setendtype}

Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant.

### setFormattingType() {#setformattingtype}

Gets or sets format type. The value of the property is ChartLineFormattingType integer constant.

### setJoinType() {#setjointype}

Specifies the joining caps. The value of the property is LineJoinType integer constant.

### setMinusValue() {#setminusvalue}

Represents negative error amount when error bar type is Custom.

### setPlusValue() {#setplusvalue}

Represents positive error amount when error bar type is Custom.

### setShowMarkerTTop() {#setshowmarkerttop}

Indicates if formatting error bars with a T-top.

### setStyle() {#setstyle}

Represents the style of the line. The value of the property is LineType integer constant.

### setThemeColor() {#setthemecolor}

Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

### setTransparency() {#settransparency}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

### setType() {#settype}

Represents error bar amount type. The value of the property is ErrorBarType integer constant.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
cells.get("C1").putValue("Q1");
cells.get("C2").putValue("Q2");
cells.get("C3").putValue("Y1");
cells.get("C4").putValue("Y2");
var chartIndex = workbook.getWorksheets().get(0).getCharts().add(aspose.cells.ChartType.COLUMN, 11, 0, 27, 10);
var chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:B4", true);
chart.getNSeries().setCategoryData("C1:C4");
for (var i = 0; i < chart.getNSeries().getCount(); i++)
{
var aseries = chart.getNSeries().get(i);
//Sets custom error bar type
aseries.getXErrorBar().setType(aspose.cells.ErrorBarType.CUSTOM);
aseries.getXErrorBar().setPlusValue("=Sheet1!A1");
aseries.getXErrorBar().setMinusValue("=Sheet1!A2");
}
```

### setVisible() {#setvisible}

Represents whether the line is visible.

### setWeight() {#setweight}

Gets or sets the WeightType of the line. The value of the property is WeightType integer constant.

### setWeightPt() {#setweightpt}

Gets or sets the weight of the line in unit of points.

### setWeightPx() {#setweightpx}

Gets or sets the weight of the line in unit of pixels.
