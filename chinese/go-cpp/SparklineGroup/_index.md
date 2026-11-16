---
title: "SparklineGroup 类"
linktitle: "SparklineGroup"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SparklineGroup 类。封装了在 Go 中表示 sparklinegroup 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> 被组织到一个 sparkline 组中。SparklineGroup 包含可变数量的 sparkline 项目。sparkline 组指定 sparkline 的类型、显示设置和轴设置。

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | 重置 sparkline 组的数据范围和位置范围。此方法将清除组中原有的 sparkline 项，并为新范围创建新的 sparkline 项。 |
| [GetPresetStyle](./getpresetstyle/) | 获取和设置 sparkline 组的预设样式类型。 |
| [SetPresetStyle](./setpresetstyle/) | 获取和设置 sparkline 组的预设样式类型。 |
| [GetSparklines](./getsparklines/) | 获取 Sparkline 对象的集合。 |
| [GetType](./gettype/) | 指示 sparkline 组的 sparkline 类型。 |
| [SetType](./settype/) | 指示 sparkline 组的 sparkline 类型。 |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | 指示如何绘制空单元格。 |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | 指示如何绘制空单元格。 |
| [GetDisplayHidden](./getdisplayhidden/) | 指示是否在隐藏的行和列中显示数据。 |
| [SetDisplayHidden](./setdisplayhidden/) | 指示是否在隐藏的行和列中显示数据。 |
| [GetShowHighPoint](./getshowhighpoint/) | 指示是否突出显示 sparkline 组中数据的最高点。 |
| [SetShowHighPoint](./setshowhighpoint/) | 指示是否突出显示 sparkline 组中数据的最高点。 |
| [GetHighPointColor](./gethighpointcolor/) | 获取和设置 sparkline 组中数据最高点的颜色。 |
| [SetHighPointColor](./sethighpointcolor/) | 获取和设置 sparkline 组中数据最高点的颜色。 |
| [GetShowLowPoint](./getshowlowpoint/) | 指示是否突出显示 sparkline 组中数据的最低点。 |
| [SetShowLowPoint](./setshowlowpoint/) | 指示是否突出显示 sparkline 组中数据的最低点。 |
| [GetLowPointColor](./getlowpointcolor/) | 获取和设置 sparkline 组中数据最低点的颜色。 |
| [SetLowPointColor](./setlowpointcolor/) | 获取和设置 sparkline 组中数据最低点的颜色。 |
| [GetShowNegativePoints](./getshownegativepoints/) | 指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。 |
| [SetShowNegativePoints](./setshownegativepoints/) | 指示是否使用不同的颜色或标记突出显示 sparkline 组中的负值。 |
| [GetNegativePointsColor](./getnegativepointscolor/) | 获取和设置 sparkline 组中负值的颜色。 |
| [SetNegativePointsColor](./setnegativepointscolor/) | 获取和设置 sparkline 组中负值的颜色。 |
| [GetShowFirstPoint](./getshowfirstpoint/) | 指示是否突出显示 sparkline 组中数据的第一个点。 |
| [SetShowFirstPoint](./setshowfirstpoint/) | 指示是否突出显示 sparkline 组中数据的第一个点。 |
| [GetFirstPointColor](./getfirstpointcolor/) | 获取和设置 sparkline 组中数据第一个点的颜色。 |
| [SetFirstPointColor](./setfirstpointcolor/) | 获取和设置 sparkline 组中数据第一个点的颜色。 |
| [GetShowLastPoint](./getshowlastpoint/) | 指示是否突出显示 sparkline 组中数据的最后一个点。 |
| [SetShowLastPoint](./setshowlastpoint/) | 指示是否突出显示 sparkline 组中数据的最后一个点。 |
| [GetLastPointColor](./getlastpointcolor/) | 获取和设置 sparkline 组中数据最后一个点的颜色。 |
| [SetLastPointColor](./setlastpointcolor/) | 获取和设置 sparkline 组中数据最后一个点的颜色。 |
| [GetShowMarkers](./getshowmarkers/) | 指示是否突出显示 sparkline 组中每条线形 sparkline 的每个点。 |
| [SetShowMarkers](./setshowmarkers/) | 指示是否突出显示 sparkline 组中每条线形 sparkline 的每个点。 |
| [GetMarkersColor](./getmarkerscolor/) | 获取和设置 sparkline 组中每条线形 sparkline 的点的颜色。 |
| [SetMarkersColor](./setmarkerscolor/) | 获取和设置 sparkline 组中每条线形 sparkline 的点的颜色。 |
| [GetSeriesColor](./getseriescolor/) | 获取和设置 sparkline 组中 sparkline 的颜色。 |
| [SetSeriesColor](./setseriescolor/) | 获取和设置 sparkline 组中 sparkline 的颜色。 |
| [GetPlotRightToLeft](./getplotrighttoleft/) | 指示绘图数据是否从右到左。 |
| [SetPlotRightToLeft](./setplotrighttoleft/) | 指示绘图数据是否从右到左。 |
| [GetLineWeight](./getlineweight/) | 获取和设置 sparkline 组中每条线形 sparkline 的线宽，单位为点。 |
| [SetLineWeight](./setlineweight/) | 获取和设置 sparkline 组中每条线形 sparkline 的线宽，单位为点。 |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | 获取并设置 sparkline 组中水平轴的颜色。 |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | 获取并设置 sparkline 组中水平轴的颜色。 |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | 指示是否显示 sparkline 水平轴。如果 sparkline 的数据跨越零轴，则会出现水平轴。 |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | 指示是否显示 sparkline 水平轴。如果 sparkline 的数据跨越零轴，则会出现水平轴。 |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | 表示包含 sparkline 数据日期值的范围。 |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | 表示包含 sparkline 数据日期值的范围。 |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | 表示垂直轴最大值类型。 |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | 表示垂直轴最大值类型。 |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | 获取并设置垂直轴的自定义最大值。 |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | 获取并设置垂直轴的自定义最大值。 |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | 使用指定的轴值类型设置 sparkline 垂直轴的自定义最大值。 |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | 使用指定的轴值类型设置 sparkline 垂直轴的自定义最小值。 |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | 表示垂直轴最小值类型。 |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | 表示垂直轴最小值类型。 |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | 获取并设置垂直轴的自定义最小值。 |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | 获取并设置垂直轴的自定义最小值。 |
