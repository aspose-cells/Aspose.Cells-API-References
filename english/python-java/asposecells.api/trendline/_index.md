---
title: "Trendline Class"
linktitle: "Trendline"
articleTitle: "Trendline"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a trendline in a chart."
type: docs
weight: 7110
url: /python-java/asposecells.api/trendline/
---

## Trendline class

Represents a trendline in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsNameAuto](#isnameauto) | boolean | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [Type](#type) | int | Returns the trendline type. The value of the property is TrendlineType integer constant. |
| [Name](#name) | String | Returns the name of the trendline. |
| [Order](#order) | int | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be |
| [Period](#period) | int | Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less |
| [Forward](#forward) | float | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of pe |
| [Backward](#backward) | float | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of p |
| [DisplayEquation](#displayequation) | boolean | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value).  |
| [DisplayRSquared](#displayrsquared) | boolean | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). S |
| [Intercept](#intercept) | float | Returns or sets the point where the trendline crosses the value axis. |
| [DataLabels](#datalabels) | DataLabels | Represents the DataLabels object for the specified series. |
| [LegendEntry](#legendentry) | LegendEntry | Gets the legend entry according to this trendline |
| [CompoundType](#compoundtype) | int | Specifies the compound line type The value of the property is MsoLineStyle integer constant. |
| [DashType](#dashtype) | int | Specifies the dash line type The value of the property is MsoLineDashStyle integer constant. |
| [CapType](#captype) | int | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [JoinType](#jointype) | int | Specifies the joining caps. The value of the property is LineJoinType integer constant. |
| [BeginType](#begintype) | int | Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [EndType](#endtype) | int | Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant. |
| [BeginArrowLength](#beginarrowlength) | int | Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer c |
| [EndArrowLength](#endarrowlength) | int | Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer con |
| [BeginArrowWidth](#beginarrowwidth) | int | Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer con |
| [EndArrowWidth](#endarrowwidth) | int | Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer const |
| [ThemeColor](#themecolor) | ThemeColor | Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned. |
| [Color](#color) | Color | Represents the com.aspose.cells.Color of the line. |
| [Transparency](#transparency) | float | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [Style](#style) | int | Represents the style of the line. The value of the property is LineType integer constant. |
| [Weight](#weight) | int | Gets or sets the WeightType of the line. The value of the property is WeightType integer constant. |
| [WeightPt](#weightpt) | float | Gets or sets the weight of the line in unit of points. |
| [WeightPx](#weightpx) | float | Gets or sets the weight of the line in unit of pixels. |
| [FormattingType](#formattingtype) | int | Gets or sets format type. The value of the property is ChartLineFormattingType integer constant. |
| [IsAutomaticColor](#isautomaticcolor) | boolean | Indicates whether the color of line is automatic assigned. |
| [IsVisible](#isvisible) | boolean | Represents whether the line is visible. |
| [IsAuto](#isauto) | boolean | Indicates whether this line style is auto assigned. |
| [GradientFill](#gradientfill) | GradientFill | Represents gradient fill. |

## Methods

| Name | Description |
| --- | --- |
| [isInterceptAuto](#isinterceptauto) | Indicates whether Microsoft Workbook automatically determines the intercept of the trendline. |
| [setInterceptAuto](#setinterceptauto) | Sets whether Microsoft Workbook automatically determines the intercept of the trendline. |

### Trendline.IsNameAuto property {#isnameauto}

Returns if Microsoft Excel automatically determines the name of the trendline.

**Type:** boolean

### Trendline.Type property {#type}

Returns the trendline type. The value of the property is TrendlineType integer constant.

**Type:** int

### Trendline.Name property {#name}

Returns the name of the trendline.

**Type:** String

### Trendline.Order property {#order}

Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.

**Type:** int

### Trendline.Period property {#period}

Returns or sets the period for the moving-average trendline. This value should be between 2 and 255. And it must be less than the number of the chart points in the series

**Type:** int

### Trendline.Forward property {#forward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.

**Type:** float

### Trendline.Backward property {#backward}

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

**Type:** float

### Trendline.DisplayEquation property {#displayequation}

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

**Type:** boolean

### Trendline.DisplayRSquared property {#displayrsquared}

Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.

**Type:** boolean

### Trendline.Intercept property {#intercept}

Returns or sets the point where the trendline crosses the value axis.

**Type:** float

### Trendline.DataLabels property {#datalabels}

Represents the DataLabels object for the specified series.

**Type:** DataLabels

### Trendline.LegendEntry property {#legendentry}

Gets the legend entry according to this trendline

**Type:** LegendEntry

### Trendline.CompoundType property {#compoundtype}

Specifies the compound line type The value of the property is MsoLineStyle integer constant.

**Type:** int

### Trendline.DashType property {#dashtype}

Specifies the dash line type The value of the property is MsoLineDashStyle integer constant.

**Type:** int

### Trendline.CapType property {#captype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

**Type:** int

### Trendline.JoinType property {#jointype}

Specifies the joining caps. The value of the property is LineJoinType integer constant.

**Type:** int

### Trendline.BeginType property {#begintype}

Specifies an arrowhead for the begin of a line. The value of the property is MsoArrowheadStyle integer constant.

**Type:** int

### Trendline.EndType property {#endtype}

Specifies an arrowhead for the end of a line. The value of the property is MsoArrowheadStyle integer constant.

**Type:** int

### Trendline.BeginArrowLength property {#beginarrowlength}

Specifies the length of the arrowhead for the begin of a line. The value of the property is MsoArrowheadLength integer constant.

**Type:** int

### Trendline.EndArrowLength property {#endarrowlength}

Specifies the length of the arrowhead for the end of a line. The value of the property is MsoArrowheadLength integer constant.

**Type:** int

### Trendline.BeginArrowWidth property {#beginarrowwidth}

Specifies the width of the arrowhead for the begin of a line. The value of the property is MsoArrowheadWidth integer constant.

**Type:** int

### Trendline.EndArrowWidth property {#endarrowwidth}

Specifies the width of the arrowhead for the end of a line. The value of the property is MsoArrowheadWidth integer constant.

**Type:** int

### Trendline.ThemeColor property {#themecolor}

Gets and sets the theme color. If the foreground color is not a theme color, NULL will be returned.

**Type:** ThemeColor

### Trendline.Color property {#color}

Represents the com.aspose.cells.Color of the line.

**Type:** Color

### Trendline.Transparency property {#transparency}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** float

### Trendline.Style property {#style}

Represents the style of the line. The value of the property is LineType integer constant.

**Type:** int

### Trendline.Weight property {#weight}

Gets or sets the WeightType of the line. The value of the property is WeightType integer constant.

**Type:** int

### Trendline.WeightPt property {#weightpt}

Gets or sets the weight of the line in unit of points.

**Type:** float

### Trendline.WeightPx property {#weightpx}

Gets or sets the weight of the line in unit of pixels.

**Type:** float

### Trendline.FormattingType property {#formattingtype}

Gets or sets format type. The value of the property is ChartLineFormattingType integer constant.

**Type:** int

### Trendline.IsAutomaticColor property {#isautomaticcolor}

Indicates whether the color of line is automatic assigned.

**Type:** boolean

### Trendline.IsVisible property {#isvisible}

Represents whether the line is visible.

**Type:** boolean

### Trendline.IsAuto property {#isauto}

Indicates whether this line style is auto assigned.

**Type:** boolean

### Trendline.GradientFill property {#gradientfill}

Represents gradient fill.

**Type:** GradientFill

### isInterceptAuto() {#isinterceptauto}

Indicates whether Microsoft Workbook automatically determines the intercept of the trendline.

### setInterceptAuto(isInterceptAuto) {#setinterceptauto}

Sets whether Microsoft Workbook automatically determines the intercept of the trendline.
