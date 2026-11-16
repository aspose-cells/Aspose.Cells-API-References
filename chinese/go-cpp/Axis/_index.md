---
title: "轴类"
linktitle: "轴"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "轴类。封装在 Go 中表示轴的对象。"
type: docs
weight: 200
url: /zh/go-cpp/axis/
---

## Axis class

封装表示图表坐标轴的对象。

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetArea](./getarea/) | 获取区域。 |
| [IsAutomaticMinValue](./isautomaticminvalue/) | 指示最小值是否自动分配。 |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | 指示最小值是否自动分配。 |
| [GetMinValue](./getminvalue/) | 表示值轴上的最小值。 |
| [SetMinValue](./setminvalue/) | 表示值轴上的最小值。 |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | 指示最大值是否自动分配。 |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | 指示最大值是否自动分配。 |
| [GetMaxValue](./getmaxvalue/) | 表示值轴上的最大值。 |
| [SetMaxValue](./setmaxvalue/) | 表示值轴上的最大值。 |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | 指示轴的主单位是否自动分配。 |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | 指示轴的主单位是否自动分配。 |
| [GetMajorUnit](./getmajorunit/) | 表示轴的主单位。 |
| [SetMajorUnit](./setmajorunit/) | 表示轴的主单位。 |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | 指示轴的次单位是否自动分配。 |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | 指示轴的次单位是否自动分配。 |
| [GetMinorUnit](./getminorunit/) | 表示轴的次单位。 |
| [SetMinorUnit](./setminorunit/) | 表示轴的次单位。 |
| [GetAxisLine](./getaxisline/) | 获取轴的外观。 |
| [GetMajorTickMark](./getmajortickmark/) | 表示指定轴的主刻度线类型。 |
| [SetMajorTickMark](./setmajortickmark/) | 表示指定轴的主刻度线类型。 |
| [GetMinorTickMark](./getminortickmark/) | 表示指定轴的次刻度线类型。 |
| [SetMinorTickMark](./setminortickmark/) | 表示指定轴的次刻度线类型。 |
| [GetTickLabelPosition](./getticklabelposition/) | 表示指定轴上刻度标签的位置。 |
| [SetTickLabelPosition](./setticklabelposition/) | 表示指定轴上刻度标签的位置。 |
| [GetCrossAt](./getcrossat/) | 表示值轴上类别轴交叉的点。 |
| [SetCrossAt](./setcrossat/) | 表示值轴上类别轴交叉的点。 |
| [GetCrossType](./getcrosstype/) | 表示指定轴上另一轴交叉的 CrossType。 |
| [SetCrossType](./setcrosstype/) | 表示指定轴上另一轴交叉的 CrossType。 |
| [GetLogBase](./getlogbase/) | 表示对数基数。默认值为 10。 |
| [SetLogBase](./setlogbase/) | 表示对数基数。默认值为 10。 |
| [IsLogarithmic](./islogarithmic/) | 表示值轴的刻度类型是否为对数。 |
| [SetIsLogarithmic](./setislogarithmic/) | 表示值轴的刻度类型是否为对数。 |
| [IsPlotOrderReversed](./isplotorderreversed/) | 表示 Microsoft Excel 是否从最后到第一绘制数据点。 |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | 表示 Microsoft Excel 是否从最后到第一绘制数据点。 |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | 表示值轴是否在类别之间跨越类别轴。 |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | 表示值轴是否在类别之间跨越类别轴。 |
| [GetTickLabels](./getticklabels/) | 返回一个 TickLabels 对象，表示指定轴的刻度标签。 |
| [GetTickLabelSpacing](./getticklabelspacing/) | 表示刻度标签之间的类别或系列数量。仅适用于类别轴和系列轴。 |
| [SetTickLabelSpacing](./setticklabelspacing/) | 表示刻度标签之间的类别或系列数量。仅适用于类别轴和系列轴。 |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | 指示刻度标签的间距是否自动 |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | 指示刻度标签的间距是否自动 |
| [GetTickMarkSpacing](./gettickmarkspacing/) | 返回或设置刻度之间的类别或系列数量。仅适用于类别轴和系列轴。 |
| [SetTickMarkSpacing](./settickmarkspacing/) | 返回或设置刻度之间的类别或系列数量。仅适用于类别轴和系列轴。 |
| [GetDisplayUnit](./getdisplayunit/) | 表示指定轴的单位标签。 |
| [SetDisplayUnit](./setdisplayunit/) | 表示指定轴的单位标签。 |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | 指定显示单位的自定义值。 |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | 指定显示单位的自定义值。 |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | 表示指定图表中轴上的单位标签。单位标签对于绘制大数值（例如百万或十亿）非常有用。 |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | 表示是否在指定轴上显示单位标签。 |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | 表示是否在指定轴上显示单位标签。 |
| [GetTitle](./gettitle/) | 获取此轴在图表中的标题。 |
| [GetCategoryType](./getcategorytype/) | 表示类别轴的类型。 |
| [SetCategoryType](./setcategorytype/) | 表示类别轴的类型。 |
| [GetBaseUnitScale](./getbaseunitscale/) | 表示类别轴的基准单位刻度。 |
| [SetBaseUnitScale](./setbaseunitscale/) | 表示类别轴的基准单位刻度。 |
| [GetMajorUnitScale](./getmajorunitscale/) | 表示类别轴的主要单位刻度。 |
| [SetMajorUnitScale](./setmajorunitscale/) | 表示类别轴的主要单位刻度。 |
| [GetMinorUnitScale](./getminorunitscale/) | 表示类别轴的主要单位刻度。 |
| [SetMinorUnitScale](./setminorunitscale/) | 表示类别轴的主要单位刻度。 |
| [IsVisible](./isvisible/) | 表示轴是否可见。 |
| [SetIsVisible](./setisvisible/) | 表示轴是否可见。 |
| [GetMajorGridLines](./getmajorgridlines/) | 表示图表轴上的主要网格线。 |
| [GetMinorGridLines](./getminorgridlines/) | 表示图表轴上的次要网格线。 |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | 指示标签是否应显示为多级。 |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | 指示标签是否应显示为多级。 |
| [GetAxisTexts](./getaxistexts/) | 在调用 Chart.Calculate() 方法后获取轴的标签。 |
| [GetBins](./getbins/) | 表示图表（直方图/帕累托）轴上的分箱。 |
