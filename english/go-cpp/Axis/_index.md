---
title: Axis Class 
linktitle: Axis
second_title: Aspose.Cells for Go via C++ API Reference
description: 'Axis class. Encapsulates the object that represents axis in Go.'
type: docs
weight: 200
url: /go-cpp/axis/
---

## Axis class

Encapsulates the object that represents an axis of chart.

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetArea](./getarea/) | Gets the Area. | 
|[IsAutomaticMinValue](./isautomaticminvalue/) | Indicates whether the min value is automatically assigned. | 
|[SetIsAutomaticMinValue](./setisautomaticminvalue/) | Indicates whether the min value is automatically assigned. | 
|[GetMinValue](./getminvalue/) | Represents the minimum value on the value axis. | 
|[SetMinValue](./setminvalue/) | Represents the minimum value on the value axis. | 
|[IsAutomaticMaxValue](./isautomaticmaxvalue/) | Indicates whether the max value is automatically assigned. | 
|[SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Indicates whether the max value is automatically assigned. | 
|[GetMaxValue](./getmaxvalue/) | Represents the maximum value on the value axis. | 
|[SetMaxValue](./setmaxvalue/) | Represents the maximum value on the value axis. | 
|[IsAutomaticMajorUnit](./isautomaticmajorunit/) | Indicates whether the major unit of the axis is automatically assigned. | 
|[SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Indicates whether the major unit of the axis is automatically assigned. | 
|[GetMajorUnit](./getmajorunit/) | Represents the major units for the axis. | 
|[SetMajorUnit](./setmajorunit/) | Represents the major units for the axis. | 
|[IsAutomaticMinorUnit](./isautomaticminorunit/) | Indicates whether the minor unit of the axis is automatically assigned. | 
|[SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Indicates whether the minor unit of the axis is automatically assigned. | 
|[GetMinorUnit](./getminorunit/) | Represents the minor units for the axis. | 
|[SetMinorUnit](./setminorunit/) | Represents the minor units for the axis. | 
|[GetAxisLine](./getaxisline/) | Gets the appearance of an Axis. | 
|[GetMajorTickMark](./getmajortickmark/) | Represents the type of major tick mark for the specified axis. | 
|[SetMajorTickMark](./setmajortickmark/) | Represents the type of major tick mark for the specified axis. | 
|[GetMinorTickMark](./getminortickmark/) | Represents the type of minor tick mark for the specified axis. | 
|[SetMinorTickMark](./setminortickmark/) | Represents the type of minor tick mark for the specified axis. | 
|[GetTickLabelPosition](./getticklabelposition/) | Represents the position of tick-mark labels on the specified axis. | 
|[SetTickLabelPosition](./setticklabelposition/) | Represents the position of tick-mark labels on the specified axis. | 
|[GetCrossAt](./getcrossat/) | Represents the point on the value axis where the category axis crosses it. | 
|[SetCrossAt](./setcrossat/) | Represents the point on the value axis where the category axis crosses it. | 
|[GetCrossType](./getcrosstype/) | Represents the CrossType on the specified axis where the other axis crosses. | 
|[SetCrossType](./setcrosstype/) | Represents the CrossType on the specified axis where the other axis crosses. | 
|[GetLogBase](./getlogbase/) | Represents the logarithmic base. Default value is 10. | 
|[SetLogBase](./setlogbase/) | Represents the logarithmic base. Default value is 10. | 
|[IsLogarithmic](./islogarithmic/) | Represents if the value axis scale type is logarithmic or not. | 
|[SetIsLogarithmic](./setislogarithmic/) | Represents if the value axis scale type is logarithmic or not. | 
|[IsPlotOrderReversed](./isplotorderreversed/) | Represents if Microsoft Excel plots data points from last to first. | 
|[SetIsPlotOrderReversed](./setisplotorderreversed/) | Represents if Microsoft Excel plots data points from last to first. | 
|[GetAxisBetweenCategories](./getaxisbetweencategories/) | Represents if the value axis crosses the category axis between categories. | 
|[SetAxisBetweenCategories](./setaxisbetweencategories/) | Represents if the value axis crosses the category axis between categories. | 
|[GetTickLabels](./getticklabels/) | Returns a TickLabels object that represents the tick-mark labels for the specified axis. | 
|[GetTickLabelSpacing](./getticklabelspacing/) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. | 
|[SetTickLabelSpacing](./setticklabelspacing/) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. | 
|[IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Indicates whether the spacing of tick label is automatic | 
|[SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Indicates whether the spacing of tick label is automatic | 
|[GetTickMarkSpacing](./gettickmarkspacing/) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. | 
|[SetTickMarkSpacing](./settickmarkspacing/) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. | 
|[GetDisplayUnit](./getdisplayunit/) | Represents the unit label for the specified axis. | 
|[SetDisplayUnit](./setdisplayunit/) | Represents the unit label for the specified axis. | 
|[GetCustomDisplayUnit](./getcustomdisplayunit/) | Specifies a custom value for the display unit. | 
|[SetCustomDisplayUnit](./setcustomdisplayunit/) | Specifies a custom value for the display unit. | 
|[GetDisplayUnitLabel](./getdisplayunitlabel/) | Represents a unit label on an axis in the specified chart.Unit labels are useful for charting large values— for example, in the millions or billions. | 
|[IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Represents if the display unit label is shown on the specified axis. | 
|[SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Represents if the display unit label is shown on the specified axis. | 
|[GetTitle](./gettitle/) | Gets the title of this axis in the chart. | 
|[GetCategoryType](./getcategorytype/) | Represents the type of the category axis. | 
|[SetCategoryType](./setcategorytype/) | Represents the type of the category axis. | 
|[GetBaseUnitScale](./getbaseunitscale/) | Represents the base unit scale for the category axis. | 
|[SetBaseUnitScale](./setbaseunitscale/) | Represents the base unit scale for the category axis. | 
|[GetMajorUnitScale](./getmajorunitscale/) | Represents the major unit scale for the category axis. | 
|[SetMajorUnitScale](./setmajorunitscale/) | Represents the major unit scale for the category axis. | 
|[GetMinorUnitScale](./getminorunitscale/) | Represents the major unit scale for the category axis. | 
|[SetMinorUnitScale](./setminorunitscale/) | Represents the major unit scale for the category axis. | 
|[IsVisible](./isvisible/) | Represents if the axis is visible. | 
|[SetIsVisible](./setisvisible/) | Represents if the axis is visible. | 
|[GetMajorGridLines](./getmajorgridlines/) | Represents major gridlines on a chart axis. | 
|[GetMinorGridLines](./getminorgridlines/) | Represents minor gridlines on a chart axis. | 
|[GetHasMultiLevelLabels](./gethasmultilevellabels/) | Indicates whether the labels shall be shown as multi level. | 
|[SetHasMultiLevelLabels](./sethasmultilevellabels/) | Indicates whether the labels shall be shown as multi level. | 
|[GetAxisTexts](./getaxistexts/) | Gets the labels of the axis after call Chart.Calculate() method. | 
|[GetBins](./getbins/) | Represents bins on a chart(Histogram/Pareto) axis | 
