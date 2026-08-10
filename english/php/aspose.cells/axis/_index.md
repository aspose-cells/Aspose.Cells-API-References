---
title: "Axis Class"
linktitle: "Axis"
articleTitle: "Axis"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents an axis of chart."
type: docs
weight: 240
url: /php/aspose.cells/axis/
---

## Axis class

Encapsulates the object that represents an axis of chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Area](#area) | Area | Gets the Area . |
| [IsAutomaticMinValue](#isautomaticminvalue) | boolean | Indicates whether the min value is automatically assigned. |
| [MinValue](#minvalue) | Object | Represents the minimum value on the value axis. The minValue type only can be double or DateTime |
| [IsAutomaticMaxValue](#isautomaticmaxvalue) | boolean | Indicates whether the max value is automatically assigned. |
| [MaxValue](#maxvalue) | Object | Represents the maximum value on the value axis. The maxValue type only can be double or DateTime |
| [IsAutomaticMajorUnit](#isautomaticmajorunit) | boolean | Indicates whether the major unit of the axis is automatically assigned. |
| [MajorUnit](#majorunit) | Number | Represents the major units for the axis. The major units must be greater than zero. |
| [IsAutomaticMinorUnit](#isautomaticminorunit) | boolean | Indicates whether the minor unit of the axis is automatically assigned. |
| [MinorUnit](#minorunit) | Number | Represents the minor units for the axis. The minor units must be greater than zero. |
| [AxisLine](#axisline) | Line | Gets the appearance of an Axis. |
| [MajorTickMark](#majortickmark) | Number | Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [MinorTickMark](#minortickmark) | Number | Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [TickLabelPosition](#ticklabelposition) | Number | Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType in |
| [CrossAt](#crossat) | Number | Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applie |
| [CrossType](#crosstype) | Number | Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType inte |
| [LogBase](#logbase) | Number | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [IsLogarithmic](#islogarithmic) | boolean | Represents if the value axis scale type is logarithmic or not. |
| [IsPlotOrderReversed](#isplotorderreversed) | boolean | Represents if Microsoft Excel plots data points from last to first. |
| [AxisBetweenCategories](#axisbetweencategories) | boolean | Represents if the value axis crosses the category axis between categories. This property applies only to category axes,  |
| [TickLabels](#ticklabels) | TickLabels | Returns a TickLabels object that represents the tick-mark labels for the specified axis. |
| [TickLabelSpacing](#ticklabelspacing) | Number | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The nu |
| [IsAutoTickLabelSpacing](#isautoticklabelspacing) | boolean | Indicates whether the spacing of tick label is automatic |
| [TickMarkSpacing](#tickmarkspacing) | Number | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The num |
| [DisplayUnit](#displayunit) | Number | Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant. |
| [CustUnit](#custunit) | Number | Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit  |
| [CustomUnit](#customunit) | Number | Specifies a custom value for the display unit. |
| [CustomDisplayUnit](#customdisplayunit) | Number |  |
| [DisplayUnitLabel](#displayunitlabel) | DisplayUnitLabel | Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example |
| [IsDisplayUnitLabelShown](#isdisplayunitlabelshown) | boolean | Represents if the display unit label is shown on the specified axis. The default value is True. |
| [Title](#title) | Title | Gets the axis' title. |
| [CategoryType](#categorytype) | Number | Represents the category axis type. The value of the property is CategoryType integer constant. |
| [BaseUnitScale](#baseunitscale) | Number | Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant. Setting th |
| [IsBaseUnitAuto](#isbaseunitauto) | boolean | Represents whether the base unit is automatic. |
| [MajorUnitScale](#majorunitscale) | Number | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [MinorUnitScale](#minorunitscale) | Number | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [IsVisible](#isvisible) | boolean | Represents if the axis is visible. |
| [MajorGridLines](#majorgridlines) | Line | Represents major gridlines on a chart axis. |
| [MinorGridLines](#minorgridlines) | Line | Represents minor gridlines on a chart axis. |
| [HasMultiLevelLabels](#hasmultilevellabels) | boolean | Indicates whether the labels shall be shown as multi level. Only valid for category axis. |
| [AxisLabels](#axislabels) | ArrayList | Gets the labels of the axis after call Chart.Calculate() method. NOTE: This member is now obsolete. Instead, please use  |
| [Bins](#bins) | AxisBins | Represents bins on a chart(Histogram/Pareto) axis |

## Methods

| Name | Description |
| --- | --- |
| [getAxisTexts](#getaxistexts) | Gets the labels of the axis after call Chart.Calculate() method. |

### Axis.Area property {#area}

Gets the Area .

**Type:** Area

### Axis.IsAutomaticMinValue property {#isautomaticminvalue}

Indicates whether the min value is automatically assigned.

**Type:** boolean

### Axis.MinValue property {#minvalue}

Represents the minimum value on the value axis. The minValue type only can be double or DateTime

**Type:** Object

### Axis.IsAutomaticMaxValue property {#isautomaticmaxvalue}

Indicates whether the max value is automatically assigned.

**Type:** boolean

### Axis.MaxValue property {#maxvalue}

Represents the maximum value on the value axis. The maxValue type only can be double or DateTime

**Type:** Object

### Axis.IsAutomaticMajorUnit property {#isautomaticmajorunit}

Indicates whether the major unit of the axis is automatically assigned.

**Type:** boolean

### Axis.MajorUnit property {#majorunit}

Represents the major units for the axis. The major units must be greater than zero.

**Type:** Number

### Axis.IsAutomaticMinorUnit property {#isautomaticminorunit}

Indicates whether the minor unit of the axis is automatically assigned.

**Type:** boolean

### Axis.MinorUnit property {#minorunit}

Represents the minor units for the axis. The minor units must be greater than zero.

**Type:** Number

### Axis.AxisLine property {#axisline}

Gets the appearance of an Axis.

**Type:** Line

### Axis.MajorTickMark property {#majortickmark}

Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constant.

**Type:** Number

### Axis.MinorTickMark property {#minortickmark}

Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constant.

**Type:** Number

### Axis.TickLabelPosition property {#ticklabelposition}

Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType integer constant.

**Type:** Number

### Axis.CrossAt property {#crossat}

Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

**Type:** Number

### Axis.CrossType property {#crosstype}

Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType integer constant.

**Type:** Number

### Axis.LogBase property {#logbase}

Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

**Type:** Number

### Axis.IsLogarithmic property {#islogarithmic}

Represents if the value axis scale type is logarithmic or not.

**Type:** boolean

### Axis.IsPlotOrderReversed property {#isplotorderreversed}

Represents if Microsoft Excel plots data points from last to first.

**Type:** boolean

### Axis.AxisBetweenCategories property {#axisbetweencategories}

Represents if the value axis crosses the category axis between categories. This property applies only to category axes, and it doesn't apply to 3-D charts.

**Type:** boolean

### Axis.TickLabels property {#ticklabels}

Returns a TickLabels object that represents the tick-mark labels for the specified axis.

**Type:** TickLabels

### Axis.TickLabelSpacing property {#ticklabelspacing}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The number must be between 1 and 31999.

**Type:** Number

### Axis.IsAutoTickLabelSpacing property {#isautoticklabelspacing}

Indicates whether the spacing of tick label is automatic

**Type:** boolean

### Axis.TickMarkSpacing property {#tickmarkspacing}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The number must be between 1 and 31999.

**Type:** Number

### Axis.DisplayUnit property {#displayunit}

Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant.

**Type:** Number

### Axis.CustUnit property {#custunit}

Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit property. This property will be removed 12 months later since January 2023. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### Axis.CustomUnit property {#customunit}

Specifies a custom value for the display unit.

**Type:** Number

### Axis.CustomDisplayUnit property {#customdisplayunit}

**Type:** Number

### Axis.DisplayUnitLabel property {#displayunitlabel}

Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

**Type:** DisplayUnitLabel

### Axis.IsDisplayUnitLabelShown property {#isdisplayunitlabelshown}

Represents if the display unit label is shown on the specified axis. The default value is True.

**Type:** boolean

### Axis.Title property {#title}

Gets the axis' title.

**Type:** Title

### Axis.CategoryType property {#categorytype}

Represents the category axis type. The value of the property is CategoryType integer constant.

**Type:** Number

### Axis.BaseUnitScale property {#baseunitscale}

Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant. Setting this property only takes effect when the CategoryType property is set to TimeScale.

**Type:** Number

### Axis.IsBaseUnitAuto property {#isbaseunitauto}

Represents whether the base unit is automatic.

**Type:** boolean

### Axis.MajorUnitScale property {#majorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Type:** Number

### Axis.MinorUnitScale property {#minorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Type:** Number

### Axis.IsVisible property {#isvisible}

Represents if the axis is visible.

**Type:** boolean

### Axis.MajorGridLines property {#majorgridlines}

Represents major gridlines on a chart axis.

**Type:** Line

### Axis.MinorGridLines property {#minorgridlines}

Represents minor gridlines on a chart axis.

**Type:** Line

### Axis.HasMultiLevelLabels property {#hasmultilevellabels}

Indicates whether the labels shall be shown as multi level. Only valid for category axis.

**Type:** boolean

### Axis.AxisLabels property {#axislabels}

Gets the labels of the axis after call Chart.Calculate() method. NOTE: This member is now obsolete. Instead, please use Axis.GetAxisTexts method. This property will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Type:** ArrayList

### Axis.Bins property {#bins}

Represents bins on a chart(Histogram/Pareto) axis

**Type:** AxisBins

### getAxisTexts() {#getaxistexts}

Gets the labels of the axis after call Chart.Calculate() method.
