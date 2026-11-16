---
title: "DataLabels 类"
linktitle: "DataLabels"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DataLabels 类。封装在 Go 中表示 datalabels 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/datalabels/
---

## DataLabels class

封装指定系列的所有 DataLabel 对象的集合。

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetBorder](./getborder/) | 获取 Line</see>。 |
| [GetArea](./getarea/) | 获取 Area</see>。 |
| [IsAutoText](./isautotext/) | 指示文本是自动生成的。 |
| [SetIsAutoText](./setisautotext/) | 指示文本是自动生成的。 |
| [GetDirectionType](./getdirectiontype/) | 获取和设置文本的方向。 |
| [SetDirectionType](./setdirectiontype/) | 获取和设置文本的方向。 |
| [GetText](./gettext/) | 获取或设置数据标签的文本。 |
| [SetText](./settext/) | 获取或设置数据标签的文本。 |
| [IsTextWrapped](./istextwrapped/) | 获取或设置指示文本是否换行的值。 |
| [SetIsTextWrapped](./setistextwrapped/) | 获取或设置指示文本是否换行的值。 |
| [GetBackgroundMode](./getbackgroundmode/) | 获取并设置背景的显示模式 |
| [SetBackgroundMode](./setbackgroundmode/) | 获取并设置背景的显示模式 |
| [GetShowValue](./getshowvalue/) | 表示指定图表的数据标签值显示行为。True 显示值，False 隐藏。 |
| [SetShowValue](./setshowvalue/) | 表示指定图表的数据标签值显示行为。True 显示值，False 隐藏。 |
| [GetShowCellRange](./getshowcellrange/) | 指示是否将单元格范围显示为数据标签。 |
| [SetShowCellRange](./setshowcellrange/) | 指示是否将单元格范围显示为数据标签。 |
| [GetShowPercentage](./getshowpercentage/) | 表示指定图表的数据标签百分比值显示行为。True 显示百分比值，False 隐藏。 |
| [SetShowPercentage](./setshowpercentage/) | 表示指定图表的数据标签百分比值显示行为。True 显示百分比值，False 隐藏。 |
| [GetShowBubbleSize](./getshowbubblesize/) | 表示指定图表的数据标签百分比值显示行为。True 显示百分比值。False 隐藏百分比值。 |
| [SetShowBubbleSize](./setshowbubblesize/) | 表示指定图表的数据标签百分比值显示行为。True 显示百分比值。False 隐藏百分比值。 |
| [GetShowCategoryName](./getshowcategoryname/) | 表示指定图表的数据标签类别名称显示行为。True 显示图表上数据标签的类别名称，False 隐藏。 |
| [SetShowCategoryName](./setshowcategoryname/) | 表示指定图表的数据标签类别名称显示行为。True 显示图表上数据标签的类别名称，False 隐藏。 |
| [GetShowSeriesName](./getshowseriesname/) | 指示系列名称是否显示在图表的数据标签上。True 显示系列名称，False 隐藏。 |
| [SetShowSeriesName](./setshowseriesname/) | 指示系列名称是否显示在图表的数据标签上。True 显示系列名称，False 隐藏。 |
| [GetShowLegendKey](./getshowlegendkey/) | 表示指定图表的数据标签图例键显示行为。如果数据标签图例键可见，则为 True。 |
| [SetShowLegendKey](./setshowlegendkey/) | 表示指定图表的数据标签图例键显示行为。如果数据标签图例键可见，则为 True。 |
| [Get_NumberFormat](./get_numberformat/) | 表示 DataLabels 对象的格式字符串。 |
| [SetNumberFormat](./setnumberformat/) | 表示 DataLabels 对象的格式字符串。 |
| [GetNumber](./getnumber/) | 获取和设置内置数字格式。 |
| [SetNumber](./setnumber/) | 获取和设置内置数字格式。 |
| [GetNumberFormatLinked](./getnumberformatlinked/) | 如果数字格式链接到单元格，则为 true（这样当单元格中的数字格式更改时，标签中的数字格式也会更改）。 |
| [SetNumberFormatLinked](./setnumberformatlinked/) | 如果数字格式链接到单元格，则为 true（这样当单元格中的数字格式更改时，标签中的数字格式也会更改）。 |
| [ApplyFont](./applyfont/) | 将数据标签的字体应用于所有子节点。 |
| [GetFont](./getfont/) | 获取 DataLabels 的字体； |
| [GetSeparatorType](./getseparatortype/) | 获取或设置图表上数据标签使用的分隔符类型。 |
| [SetSeparatorType](./setseparatortype/) | 获取或设置图表上数据标签使用的分隔符类型。 |
| [GetSeparatorValue](./getseparatorvalue/) | 获取或设置用于图表数据标签的分隔符值。 |
| [SetSeparatorValue](./setseparatorvalue/) | 获取或设置用于图表数据标签的分隔符值。 |
| [GetPosition](./getposition/) | 表示数据标签的位置。 |
| [SetPosition](./setposition/) | 表示数据标签的位置。 |
| [IsNeverOverlap](./isneveroverlap/) | 指示在将饼图转换为图像时数据标签是否永不重叠。注意：此属性仅在将饼图转换为图像时有意义。 |
| [SetIsNeverOverlap](./setisneveroverlap/) | 指示在将饼图转换为图像时数据标签是否永不重叠。注意：此属性仅在将饼图转换为图像时有意义。 |
| [GetShapeType](./getshapetype/) | 获取或设置数据标签的形状类型。 |
| [SetShapeType](./setshapetype/) | 获取或设置数据标签的形状类型。 |
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
| [GetTextOptions](./gettextoptions/) | 获取或设置文本的选项。 |
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
| [GetLinkedSource](./getlinkedsource/) | 获取和设置对工作表的引用。 |
| [SetLinkedSource](./setlinkedsource/) | 获取和设置对工作表的引用。 |
