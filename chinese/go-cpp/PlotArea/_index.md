---
title: "PlotArea 类"
linktitle: "PlotArea"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PlotArea 类。封装了在 Go 中表示 plotArea 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/plotarea/
---

## PlotArea class

封装表示图表中绘图区域的对象。

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPlotArea](./newplotarea/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetXRatioToChart](./getxratiotochart/) | 获取或设置绘图区域边界框左上角的 x 坐标，作为图表区域的比例。 |
| [SetXRatioToChart](./setxratiotochart/) | 获取或设置绘图区域边界框左上角的 x 坐标，作为图表区域的比例。 |
| [GetYRatioToChart](./getyratiotochart/) | 获取或设置绘图区域边界框左上角的 y 坐标，作为图表区域的比例。 |
| [SetYRatioToChart](./setyratiotochart/) | 获取或设置绘图区域边界框左上角的 y 坐标，作为图表区域的比例。 |
| [GetHeightRatioToChart](./getheightratiotochart/) | 获取或设置绘图区域边界框的高度，单位为图表区域比例。 |
| [SetHeightRatioToChart](./setheightratiotochart/) | 获取或设置绘图区域边界框的高度，单位为图表区域比例。 |
| [GetWidthRatioToChart](./getwidthratiotochart/) | 获取或设置绘图区域边界框的宽度，单位为图表区域比例。 |
| [SetWidthRatioToChart](./setwidthratiotochart/) | 获取或设置绘图区域边界框的宽度，单位为图表区域比例。 |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | 获取或获取绘图区域左上角的 x 坐标，单位为图表区域比例。 |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | 获取或获取绘图区域左上角的 x 坐标，单位为图表区域比例。 |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | 获取或获取绘图区域左上角的 x 坐标，单位为图表区域比例。 |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | 获取或获取绘图区域左上角的 x 坐标，单位为图表区域比例。 |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | 获取或设置绘图区域的高度，单位为图表区域比例。 |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | 获取或设置绘图区域的高度，单位为图表区域比例。 |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | 获取或设置绘图区域的宽度，单位为图表区域的比例。 |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | 获取或设置绘图区域的宽度，单位为图表区域的比例。 |
| [SetPositionAuto](./setpositionauto/) | 将绘图区域的位置设置为自动 |
| [IsAutomaticSize](./isautomaticsize/) | 指示绘图区域是否自动调整大小。 |
| [SetIsAutomaticSize](./setisautomaticsize/) | 指示绘图区域是否自动调整大小。 |
| [IsInnerMode](./isinnermode/) | 指示绘图区域的大小是否包括刻度线和轴标签。False 表示大小应决定绘图区域、刻度线和轴标签的尺寸。 |
| [SetIsInnerMode](./setisinnermode/) | 指示绘图区域的大小是否包括刻度线和轴标签。False 表示大小应决定绘图区域、刻度线和轴标签的尺寸。 |
| [GetShadow](./getshadow/) | 如果框架有阴影，则为 True。 |
| [SetShadow](./setshadow/) | 如果框架有阴影，则为 True。 |
| [GetShapeProperties](./getshapeproperties/) | 获取 ShapeProperties 对象。 |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | 指示是否已设置默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | 表示默认位置的 x，单位为图表区域的比例。 |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | 表示默认位置的 y，单位为图表区域的比例。 |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | 表示默认位置的宽度，单位为图表区域的比例。 |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | 表示默认位置的高度，单位为图表区域的比例。 |
| [GetBorder](./getborder/) | 获取 Line</see>。 |
| [GetArea](./getarea/) | 获取 Area</see>。 |
| [GetTextOptions](./gettextoptions/) | 获取或设置文本的选项。 |
| [GetFont](./getfont/) | 获取指定 ChartFrame 对象的 Font 对象。 |
| [GetAutoScaleFont](./getautoscalefont/) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。 |
| [SetAutoScaleFont](./setautoscalefont/) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。 |
| [GetXPixel](./getxpixel/) | 获取或设置左上角的 x 坐标，单位为像素。 |
| [SetXPixel](./setxpixel/) | 获取或设置左上角的 x 坐标，单位为像素。 |
| [GetYPixel](./getypixel/) | 获取或设置左上角的 y 坐标，单位为像素。 |
| [SetYPixel](./setypixel/) | 获取或设置左上角的 y 坐标，单位为像素。 |
| [GetWidthPixel](./getwidthpixel/) | 获取或设置框架的宽度，单位为像素。 |
| [SetWidthPixel](./setwidthpixel/) | 获取或设置框架的宽度，单位为像素。 |
| [GetHeightPixel](./getheightpixel/) | 获取或设置框架的高度，单位为像素。 |
| [SetHeightPixel](./setheightpixel/) | 获取或设置框架的高度，单位为像素。 |
