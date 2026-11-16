---
title: "ChartTextFrame 类"
linktitle: "ChartTextFrame"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ChartTextFrame 类。封装在 Go 中表示 charttextframe 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/charttextframe/
---

## ChartTextFrame class

封装表示包含文本的框架对象的对象。

```go

type ChartTextFrame struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewChartTextFrame](./newcharttextframe/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsDeleted](./isdeleted/) | 指示此数据标签是否已删除。 |
| [SetIsDeleted](./setisdeleted/) | 指示此数据标签是否已删除。 |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | 获取和设置文本的水平对齐方式。 |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | 获取和设置文本的水平对齐方式。 |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | 获取或设置文本的垂直对齐方式。 |
| [SetTextVerticalAlignment](./settextverticalalignment/) | 获取或设置文本的垂直对齐方式。 |
| [GetRotationAngle](./getrotationangle/) | 表示文本的旋转角度。 |
| [SetRotationAngle](./setrotationangle/) | 表示文本的旋转角度。 |
| [IsAutomaticRotation](./isautomaticrotation/) | 指示图表的文本是否自动旋转。 |
| [Characters](./characters/) | 返回表示文本中字符范围的 Characters 对象。 |
| [GetReadingOrder](./getreadingorder/) | 表示文本的阅读顺序。 |
| [SetReadingOrder](./setreadingorder/) | 表示文本的阅读顺序。 |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | 获取或设置形状是否应自动适配以完整容纳其中描述的文本。自动适配是指在形状内的文本被缩放以容纳所有文本。 |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | 获取或设置形状是否应自动适配以完整容纳其中描述的文本。自动适配是指在形状内的文本被缩放以容纳所有文本。 |
| [IsAutoText](./isautotext/) | 指示文本是自动生成的。 |
| [SetIsAutoText](./setisautotext/) | 指示文本是自动生成的。 |
| [GetText](./gettext/) | 获取或设置框架标题的文本。 |
| [SetText](./settext/) | 获取或设置框架标题的文本。 |
| [GetLinkedSource](./getlinkedsource/) | 获取和设置对工作表的引用。 |
| [SetLinkedSource](./setlinkedsource/) | 获取和设置对工作表的引用。 |
| [GetDirectionType](./getdirectiontype/) | 获取和设置文本的方向。 |
| [SetDirectionType](./setdirectiontype/) | 获取和设置文本的方向。 |
| [IsTextWrapped](./istextwrapped/) | 获取或设置指示文本是否换行的值。 |
| [SetIsTextWrapped](./setistextwrapped/) | 获取或设置指示文本是否换行的值。 |
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
| [IsAutomaticSize](./isautomaticsize/) | 指示图表框架是否自动调整大小。 |
| [SetIsAutomaticSize](./setisautomaticsize/) | 指示图表框架是否自动调整大小。 |
| [GetXRatioToChart](./getxratiotochart/) | 获取或设置左上角的 x 坐标，单位为图表区域的比例。 |
| [SetXRatioToChart](./setxratiotochart/) | 获取或设置左上角的 x 坐标，单位为图表区域的比例。 |
| [GetYRatioToChart](./getyratiotochart/) | 获取或设置左上角的 y 坐标，单位为图表区域的比例。 |
| [SetYRatioToChart](./setyratiotochart/) | 获取或设置左上角的 y 坐标，单位为图表区域的比例。 |
| [GetWidthRatioToChart](./getwidthratiotochart/) | 获取或设置框架的宽度，单位为图表区域的比例。 |
| [SetWidthRatioToChart](./setwidthratiotochart/) | 获取或设置框架的宽度，单位为图表区域的比例。 |
| [GetHeightRatioToChart](./getheightratiotochart/) | 获取或设置框架的高度，单位为图表区域的比例。 |
| [SetHeightRatioToChart](./setheightratiotochart/) | 获取或设置框架的高度，单位为图表区域的比例。 |
| [GetXPixel](./getxpixel/) | 获取或设置左上角的 x 坐标，单位为像素。 |
| [SetXPixel](./setxpixel/) | 获取或设置左上角的 x 坐标，单位为像素。 |
| [GetYPixel](./getypixel/) | 获取或设置左上角的 y 坐标，单位为像素。 |
| [SetYPixel](./setypixel/) | 获取或设置左上角的 y 坐标，单位为像素。 |
| [GetWidthPixel](./getwidthpixel/) | 获取或设置框架的宽度，单位为像素。 |
| [SetWidthPixel](./setwidthpixel/) | 获取或设置框架的宽度，单位为像素。 |
| [GetHeightPixel](./getheightpixel/) | 获取或设置框架的高度，单位为像素。 |
| [SetHeightPixel](./setheightpixel/) | 获取或设置框架的高度，单位为像素。 |
| [SetPositionAuto](./setpositionauto/) | 将框架位置设置为自动 |
