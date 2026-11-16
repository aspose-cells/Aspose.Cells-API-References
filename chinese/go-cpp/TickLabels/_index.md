---
title: "TickLabels 类"
linktitle: "TickLabels"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TickLabels 类。封装了在 Go 中表示 ticklabels 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/ticklabels/
---

## TickLabels class

表示与图表坐标轴刻度线关联的刻度标签。

```go

type TickLabels struct  {
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
| [GetFont](./getfont/) | 返回一个 Font 对象，表示指定 TickLabels 对象的字体。 |
| [GetAutoScaleFont](./getautoscalefont/) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。 |
| [SetAutoScaleFont](./setautoscalefont/) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。 |
| [GetBackgroundMode](./getbackgroundmode/) | 获取并设置背景的显示模式 |
| [SetBackgroundMode](./setbackgroundmode/) | 获取并设置背景的显示模式 |
| [GetRotationAngle](./getrotationangle/) | 表示文本顺时针旋转角度。 |
| [SetRotationAngle](./setrotationangle/) | 表示文本顺时针旋转角度。 |
| [IsAutomaticRotation](./isautomaticrotation/) | 指示旋转角度是否自动。 |
| [SetIsAutomaticRotation](./setisautomaticrotation/) | 指示旋转角度是否自动。 |
| [Get_NumberFormat](./get_numberformat/) | 表示 TickLabels 对象的格式字符串。 |
| [SetNumberFormat](./setnumberformat/) | 表示 TickLabels 对象的格式字符串。 |
| [GetNumber](./getnumber/) | 表示 TickLabels 对象的格式编号。 |
| [SetNumber](./setnumber/) | 表示 TickLabels 对象的格式编号。 |
| [GetNumberFormatLinked](./getnumberformatlinked/) | 如果数字格式链接到单元格，则为 true（这样当单元格中的数字格式更改时，标签中的数字格式也会更改）。 |
| [SetNumberFormatLinked](./setnumberformatlinked/) | 如果数字格式链接到单元格，则为 true（这样当单元格中的数字格式更改时，标签中的数字格式也会更改）。 |
| [GetDisplayNumberFormat](./getdisplaynumberformat/) | 获取和设置刻度标签的显示数字格式。 |
| [GetOffset](./getoffset/) | 获取和设置标签与分类轴的距离。仅适用于分类（x）轴。 |
| [SetOffset](./setoffset/) | 获取和设置标签与分类轴的距离。仅适用于分类（x）轴。 |
| [GetReadingOrder](./getreadingorder/) | 表示文本的阅读顺序。 |
| [SetReadingOrder](./setreadingorder/) | 表示文本的阅读顺序。 |
| [GetDirectionType](./getdirectiontype/) | 获取和设置文本的方向。 |
| [SetDirectionType](./setdirectiontype/) | 获取和设置文本的方向。 |
| [GetTickLabelItems](./getticklabelitems/) | 获取轴的显示刻度标签。 |
| [GetAlignmentType](./getalignmenttype/) | 获取和设置轴上刻度标签的文本对齐方式。 |
| [SetAlignmentType](./setalignmenttype/) | 获取和设置轴上刻度标签的文本对齐方式。 |
