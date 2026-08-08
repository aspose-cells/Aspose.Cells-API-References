---
title: "Axis"
linktitle: "Axis"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents an axis of chart."
type: docs
weight: 180
url: /nodejs/aspose.cells/axis/
---

## Axis class

Encapsulates the object that represents an axis of chart.

## Methods

| Name | Description |
| --- | --- |
| [getArea()](#getarea) | Gets the Area. |
| [getAxisBetweenCategories()](#getaxisbetweencategories) | Represents if the value axis crosses the category axis between categories. This property applies only to category axes,  |
| [getAxisLabels()](#getaxislabels) | Gets the labels of the axis after call Chart.Calculate() method. NOTE: This member is now obsolete. Instead, please use  |
| [getAxisLine()](#getaxisline) | Gets the appearance of an Axis. |
| [getAxisTexts()](#getaxistexts) | Gets the labels of the axis after call Chart.Calculate() method. |
| [getBaseUnitScale()](#getbaseunitscale) | Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant.Setting thi |
| [getBins()](#getbins) | Represents bins on a chart(Histogram/Pareto) axis |
| [getCategoryType()](#getcategorytype) | Represents the category axis type. The value of the property is CategoryType integer constant. |
| [getCrossAt()](#getcrossat) | Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applie |
| [getCrossType()](#getcrosstype) | Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType inte |
| [getCustUnit()](#getcustunit) | Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit  |
| [getCustomDisplayUnit()](#getcustomdisplayunit) |  |
| [getCustomUnit()](#getcustomunit) | Specifies a custom value for the display unit. |
| [getDisplayUnit()](#getdisplayunit) | Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant. |
| [getDisplayUnitLabel()](#getdisplayunitlabel) | Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example |
| [getLogBase()](#getlogbase) | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [getMajorGridLines()](#getmajorgridlines) | Represents major gridlines on a chart axis. |
| [getMajorTickMark()](#getmajortickmark) | Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [getMajorUnit()](#getmajorunit) | Represents the major units for the axis. The major units must be greater than zero. |
| [getMajorUnitScale()](#getmajorunitscale) | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [getMaxValue()](#getmaxvalue) | Represents the maximum value on the value axis. The maxValue type only can be double or DateTime |
| [getMinValue()](#getminvalue) | Represents the minimum value on the value axis. The minValue type only can be double or DateTime |
| [getMinorGridLines()](#getminorgridlines) | Represents minor gridlines on a chart axis. |
| [getMinorTickMark()](#getminortickmark) | Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [getMinorUnit()](#getminorunit) | Represents the minor units for the axis. The minor units must be greater than zero. |
| [getMinorUnitScale()](#getminorunitscale) | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [getTickLabelPosition()](#getticklabelposition) | Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType in |
| [getTickLabelSpacing()](#getticklabelspacing) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The nu |
| [getTickLabels()](#getticklabels) | Returns a TickLabels object that represents the tick-mark labels for the specified axis. |
| [getTickMarkSpacing()](#gettickmarkspacing) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The num |
| [getTitle()](#gettitle) | Gets the axis' title. |
| [hasMultiLevelLabels()](#hasmultilevellabels) | Indicates whether the labels shall be shown as multi level. Only valid for category axis. |
| [isAutoTickLabelSpacing()](#isautoticklabelspacing) | Indicates whether the spacing of tick label is automatic |
| [isAutomaticMajorUnit()](#isautomaticmajorunit) | Indicates whether the major unit of the axis is automatically assigned. |
| [isAutomaticMaxValue()](#isautomaticmaxvalue) | Indicates whether the max value is automatically assigned. |
| [isAutomaticMinValue()](#isautomaticminvalue) | Indicates whether the min value is automatically assigned. |
| [isAutomaticMinorUnit()](#isautomaticminorunit) | Indicates whether the minor unit of the axis is automatically assigned. |
| [isBaseUnitAuto()](#isbaseunitauto) | Represents whether the base unit is automatic. |
| [isDisplayUnitLabelShown()](#isdisplayunitlabelshown) | Represents if the display unit label is shown on the specified axis. The default value is True. |
| [isLogarithmic()](#islogarithmic) | Represents if the value axis scale type is logarithmic or not. |
| [isPlotOrderReversed()](#isplotorderreversed) | Represents if Microsoft Excel plots data points from last to first. |
| [isVisible()](#isvisible) | Represents if the axis is visible. |
| [setAutoTickLabelSpacing()](#setautoticklabelspacing) | Indicates whether the spacing of tick label is automatic |
| [setAutomaticMajorUnit()](#setautomaticmajorunit) | Indicates whether the major unit of the axis is automatically assigned. |
| [setAutomaticMaxValue()](#setautomaticmaxvalue) | Indicates whether the max value is automatically assigned. |
| [setAutomaticMinValue()](#setautomaticminvalue) | Indicates whether the min value is automatically assigned. |
| [setAutomaticMinorUnit()](#setautomaticminorunit) | Indicates whether the minor unit of the axis is automatically assigned. |
| [setAxisBetweenCategories()](#setaxisbetweencategories) | Represents if the value axis crosses the category axis between categories. This property applies only to category axes,  |
| [setBaseUnitAuto()](#setbaseunitauto) | Represents whether the base unit is automatic. |
| [setBaseUnitScale()](#setbaseunitscale) | Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant.Setting thi |
| [setCategoryType()](#setcategorytype) | Represents the category axis type. The value of the property is CategoryType integer constant. |
| [setCrossAt()](#setcrossat) | Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applie |
| [setCrossType()](#setcrosstype) | Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType inte |
| [setCustUnit()](#setcustunit) | Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit  |
| [setCustomDisplayUnit()](#setcustomdisplayunit) |  |
| [setCustomUnit()](#setcustomunit) | Specifies a custom value for the display unit. |
| [setDisplayUnit()](#setdisplayunit) | Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant. |
| [setDisplayUnitLabelShown()](#setdisplayunitlabelshown) | Represents if the display unit label is shown on the specified axis. The default value is True. |
| [setHasMultiLevelLabels()](#sethasmultilevellabels) | Indicates whether the labels shall be shown as multi level. Only valid for category axis. |
| [setLogBase()](#setlogbase) | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [setLogarithmic()](#setlogarithmic) | Represents if the value axis scale type is logarithmic or not. |
| [setMajorTickMark()](#setmajortickmark) | Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [setMajorUnit()](#setmajorunit) | Represents the major units for the axis. The major units must be greater than zero. |
| [setMajorUnitScale()](#setmajorunitscale) | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [setMaxValue()](#setmaxvalue) | Represents the maximum value on the value axis. The maxValue type only can be double or DateTime |
| [setMinValue()](#setminvalue) | Represents the minimum value on the value axis. The minValue type only can be double or DateTime |
| [setMinorTickMark()](#setminortickmark) | Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constan |
| [setMinorUnit()](#setminorunit) | Represents the minor units for the axis. The minor units must be greater than zero. |
| [setMinorUnitScale()](#setminorunitscale) | Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant. |
| [setPlotOrderReversed()](#setplotorderreversed) | Represents if Microsoft Excel plots data points from last to first. |
| [setTickLabelPosition()](#setticklabelposition) | Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType in |
| [setTickLabelSpacing()](#setticklabelspacing) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The nu |
| [setTickMarkSpacing()](#settickmarkspacing) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The num |
| [setVisible()](#setvisible) | Represents if the axis is visible. |

### getArea() {#getarea}

Gets the Area.

### getAxisBetweenCategories() {#getaxisbetweencategories}

Represents if the value axis crosses the category axis between categories. This property applies only to category axes, and it doesn't apply to 3-D charts.

### getAxisLabels() {#getaxislabels}

Gets the labels of the axis after call Chart.Calculate() method. NOTE: This member is now obsolete. Instead, please use Axis.GetAxisTexts method. This property will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

### getAxisLine() {#getaxisline}

Gets the appearance of an Axis.

### getAxisTexts() {#getaxistexts}

Gets the labels of the axis after call Chart.Calculate() method.

### getBaseUnitScale() {#getbaseunitscale}

Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant.Setting this property only takes effect when the CategoryType property is set to TimeScale.

### getBins() {#getbins}

Represents bins on a chart(Histogram/Pareto) axis

### getCategoryType() {#getcategorytype}

Represents the category axis type. The value of the property is CategoryType integer constant.

### getCrossAt() {#getcrossat}

Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### getCrossType() {#getcrosstype}

Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType integer constant.

### getCustUnit() {#getcustunit}

Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit property. This property will be removed 12 months later since January 2023. Aspose apologizes for any inconvenience you may have experienced.

### getCustomDisplayUnit() {#getcustomdisplayunit}

### getCustomUnit() {#getcustomunit}

Specifies a custom value for the display unit.

### getDisplayUnit() {#getdisplayunit}

Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant.

### getDisplayUnitLabel() {#getdisplayunitlabel}

Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

### getLogBase() {#getlogbase}

Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

### getMajorGridLines() {#getmajorgridlines}

Represents major gridlines on a chart axis.

**Example:**

```js
chart.getValueAxis().getMajorGridLines().setVisible(false);
chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

### getMajorTickMark() {#getmajortickmark}

Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constant.

### getMajorUnit() {#getmajorunit}

Represents the major units for the axis. The major units must be greater than zero.

### getMajorUnitScale() {#getmajorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Example:**

```js
chart.getCategoryAxis().setCategoryType(aspose.cells.CategoryType.TIME_SCALE);
chart.getCategoryAxis().setMajorUnitScale(aspose.cells.TimeUnit.MONTHS);
chart.getCategoryAxis().setMajorUnit(2);
```

### getMaxValue() {#getmaxvalue}

Represents the maximum value on the value axis. The maxValue type only can be double or DateTime

### getMinValue() {#getminvalue}

Represents the minimum value on the value axis. The minValue type only can be double or DateTime

### getMinorGridLines() {#getminorgridlines}

Represents minor gridlines on a chart axis.

### getMinorTickMark() {#getminortickmark}

Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constant.

### getMinorUnit() {#getminorunit}

Represents the minor units for the axis. The minor units must be greater than zero.

### getMinorUnitScale() {#getminorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Example:**

```js
chart.getCategoryAxis().setCategoryType(aspose.cells.CategoryType.TIME_SCALE);
chart.getCategoryAxis().setMinorUnitScale(aspose.cells.TimeUnit.MONTHS);
chart.getCategoryAxis().setMinorUnit(2);
```

### getTickLabelPosition() {#getticklabelposition}

Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType integer constant.

### getTickLabelSpacing() {#getticklabelspacing}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The number must be between 1 and 31999.

### getTickLabels() {#getticklabels}

Returns a TickLabels object that represents the tick-mark labels for the specified axis.

### getTickMarkSpacing() {#gettickmarkspacing}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The number must be between 1 and 31999.

### getTitle() {#gettitle}

Gets the axis' title.

### hasMultiLevelLabels() {#hasmultilevellabels}

Indicates whether the labels shall be shown as multi level. Only valid for category axis.

### isAutoTickLabelSpacing() {#isautoticklabelspacing}

Indicates whether the spacing of tick label is automatic

### isAutomaticMajorUnit() {#isautomaticmajorunit}

Indicates whether the major unit of the axis is automatically assigned.

### isAutomaticMaxValue() {#isautomaticmaxvalue}

Indicates whether the max value is automatically assigned.

### isAutomaticMinValue() {#isautomaticminvalue}

Indicates whether the min value is automatically assigned.

### isAutomaticMinorUnit() {#isautomaticminorunit}

Indicates whether the minor unit of the axis is automatically assigned.

### isBaseUnitAuto() {#isbaseunitauto}

Represents whether the base unit is automatic.

### isDisplayUnitLabelShown() {#isdisplayunitlabelshown}

Represents if the display unit label is shown on the specified axis. The default value is True.

### isLogarithmic() {#islogarithmic}

Represents if the value axis scale type is logarithmic or not.

### isPlotOrderReversed() {#isplotorderreversed}

Represents if Microsoft Excel plots data points from last to first.

### isVisible() {#isvisible}

Represents if the axis is visible.

### setAutoTickLabelSpacing() {#setautoticklabelspacing}

Indicates whether the spacing of tick label is automatic

### setAutomaticMajorUnit() {#setautomaticmajorunit}

Indicates whether the major unit of the axis is automatically assigned.

### setAutomaticMaxValue() {#setautomaticmaxvalue}

Indicates whether the max value is automatically assigned.

### setAutomaticMinValue() {#setautomaticminvalue}

Indicates whether the min value is automatically assigned.

### setAutomaticMinorUnit() {#setautomaticminorunit}

Indicates whether the minor unit of the axis is automatically assigned.

### setAxisBetweenCategories() {#setaxisbetweencategories}

Represents if the value axis crosses the category axis between categories. This property applies only to category axes, and it doesn't apply to 3-D charts.

### setBaseUnitAuto() {#setbaseunitauto}

Represents whether the base unit is automatic.

### setBaseUnitScale() {#setbaseunitscale}

Represents the base unit scale for the category axis. The value of the property is TimeUnit integer constant.Setting this property only takes effect when the CategoryType property is set to TimeScale.

### setCategoryType() {#setcategorytype}

Represents the category axis type. The value of the property is CategoryType integer constant.

### setCrossAt() {#setcrossat}

Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### setCrossType() {#setcrosstype}

Represents the CrossType on the specified axis where the other axis crosses. The value of the property is CrossType integer constant.

### setCustUnit() {#setcustunit}

Specifies a custom value for the display unit. NOTE: This property is now obsolete. Instead, please use Axis.CustomUnit property. This property will be removed 12 months later since January 2023. Aspose apologizes for any inconvenience you may have experienced.

### setCustomDisplayUnit() {#setcustomdisplayunit}

### setCustomUnit() {#setcustomunit}

Specifies a custom value for the display unit.

### setDisplayUnit() {#setdisplayunit}

Represents the unit label for the specified axis. The value of the property is DisplayUnitType integer constant.

### setDisplayUnitLabelShown() {#setdisplayunitlabelshown}

Represents if the display unit label is shown on the specified axis. The default value is True.

### setHasMultiLevelLabels() {#sethasmultilevellabels}

Indicates whether the labels shall be shown as multi level. Only valid for category axis.

### setLogBase() {#setlogbase}

Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

### setLogarithmic() {#setlogarithmic}

Represents if the value axis scale type is logarithmic or not.

### setMajorTickMark() {#setmajortickmark}

Represents the type of major tick mark for the specified axis. The value of the property is TickMarkType integer constant.

### setMajorUnit() {#setmajorunit}

Represents the major units for the axis. The major units must be greater than zero.

### setMajorUnitScale() {#setmajorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Example:**

```js
chart.getCategoryAxis().setCategoryType(aspose.cells.CategoryType.TIME_SCALE);
chart.getCategoryAxis().setMajorUnitScale(aspose.cells.TimeUnit.MONTHS);
chart.getCategoryAxis().setMajorUnit(2);
```

### setMaxValue() {#setmaxvalue}

Represents the maximum value on the value axis. The maxValue type only can be double or DateTime

### setMinValue() {#setminvalue}

Represents the minimum value on the value axis. The minValue type only can be double or DateTime

### setMinorTickMark() {#setminortickmark}

Represents the type of minor tick mark for the specified axis. The value of the property is TickMarkType integer constant.

### setMinorUnit() {#setminorunit}

Represents the minor units for the axis. The minor units must be greater than zero.

### setMinorUnitScale() {#setminorunitscale}

Represents the major unit scale for the category axis. The value of the property is TimeUnit integer constant.

**Example:**

```js
chart.getCategoryAxis().setCategoryType(aspose.cells.CategoryType.TIME_SCALE);
chart.getCategoryAxis().setMinorUnitScale(aspose.cells.TimeUnit.MONTHS);
chart.getCategoryAxis().setMinorUnit(2);
```

### setPlotOrderReversed() {#setplotorderreversed}

Represents if Microsoft Excel plots data points from last to first.

### setTickLabelPosition() {#setticklabelposition}

Represents the position of tick-mark labels on the specified axis. The value of the property is TickLabelPositionType integer constant.

### setTickLabelSpacing() {#setticklabelspacing}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The number must be between 1 and 31999.

### setTickMarkSpacing() {#settickmarkspacing}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The number must be between 1 and 31999.

### setVisible() {#setvisible}

Represents if the axis is visible.
