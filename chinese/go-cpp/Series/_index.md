---
title: "Series 类"
linktitle: "Series"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Series 类。封装在 Go 中表示 series 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/series/
---

## Series class

封装表示图表中单个数据系列的对象。

```go

type Series struct  {
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
| [IsFiltered](./isfiltered/) | 指示系列是否被选中或过滤。True 表示该系列已被过滤，它将不会在图表中显示。 |
| [SetIsFiltered](./setisfiltered/) | 指示系列是否被选中或过滤。True 表示该系列已被过滤，它将不会在图表中显示。 |
| [GetLayoutProperties](./getlayoutproperties/) | 表示布局的属性。 |
| [Move](./move/) | 上下移动系列。 |
| [GetPoints](./getpoints/) | 获取图表中系列的点集合。 |
| [GetArea](./getarea/) | 表示 Series 对象的背景区域。 |
| [GetBorder](./getborder/) | 表示 Series 对象的边框。 |
| [GetName](./getname/) | 获取或设置数据系列的名称。 |
| [SetName](./setname/) | 获取或设置数据系列的名称。 |
| [GetDisplayName](./getdisplayname/) | 获取显示在图表上的系列名称。 |
| [GetCountOfDataValues](./getcountofdatavalues/) | 获取数据值的数量。 |
| [IsVerticalValues](./isverticalvalues/) | 指示数据源是否为垂直方向。 |
| [GetValues](./getvalues/) | 表示此图表系列的 Y 值。 |
| [SetValues](./setvalues/) | 表示此图表系列的 Y 值。 |
| [GetPointValues](./getpointvalues/) | 获取用于在图表中绘制此系列每个点的实际值。 |
| [GetCategoryValues](./getcategoryvalues/) | 获取用于在图表中绘制此系列每个点的实际类别值。 |
| [GetValuesFormatCode](./getvaluesformatcode/) | 表示 Values NumberList 的格式代码。 |
| [SetValuesFormatCode](./setvaluesformatcode/) | 表示 Values NumberList 的格式代码。 |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | 表示 X Values 的 NumberList 的格式代码。 |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | 表示 X Values 的 NumberList 的格式代码。 |
| [GetXValues](./getxvalues/) | 表示此图表系列的 X 值。 |
| [SetXValues](./setxvalues/) | 表示此图表系列的 X 值。 |
| [GetBubbleSizes](./getbubblesizes/) | 获取或设置图表系列的气泡大小值。 |
| [SetBubbleSizes](./setbubblesizes/) | 获取或设置图表系列的气泡大小值。 |
| [GetTrendLines](./gettrendlines/) | 返回此系列的所有趋势线。 |
| [GetSmooth](./getsmooth/) | 表示曲线平滑。True 表示已为折线图或散点图启用曲线平滑。仅适用于折线图和带线的散点图。 |
| [SetSmooth](./setsmooth/) | 表示曲线平滑。True 表示已为折线图或散点图启用曲线平滑。仅适用于折线图和带线的散点图。 |
| [GetShadow](./getshadow/) | 若系列具有阴影，则为 True。 |
| [SetShadow](./setshadow/) | 若系列具有阴影，则为 True。 |
| [GetHas3DEffect](./gethas3deffect/) | 若系列具有三维外观，则为 True。 |
| [SetHas3DEffect](./sethas3deffect/) | 若系列具有三维外观，则为 True。 |
| [GetBar3DShapeType](./getbar3dshapetype/) | 获取或设置用于 3-D 条形图或柱形图的 3D 形状类型。 |
| [SetBar3DShapeType](./setbar3dshapetype/) | 获取或设置用于 3-D 条形图或柱形图的 3D 形状类型。 |
| [GetDataLabels](./getdatalabels/) | 表示指定 ASeries 的 DataLabels 对象。 |
| [GetType](./gettype/) | 获取或设置数据系列的类型。 |
| [SetType](./settype/) | 获取或设置数据系列的类型。 |
| [GetMarker](./getmarker/) | 获取 Marker。 |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | 指示此系列是否绘制在第二值轴上。 |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | 指示此系列是否绘制在第二值轴上。 |
| [GetXErrorBar](./getxerrorbar/) | 表示系列的 X 方向误差棒。 |
| [GetYErrorBar](./getyerrorbar/) | 表示系列的 Y 方向误差棒。 |
| [GetHasHiLoLines](./gethashilolines/) | 若折线图具有高低线，则为 True。仅适用于折线图。 |
| [SetHasHiLoLines](./sethashilolines/) | 若折线图具有高低线，则为 True。仅适用于折线图。 |
| [GetHiLoLines](./gethilolines/) | 返回一个 HiLoLines 对象，表示折线图中系列的高低线。仅适用于折线图。 |
| [GetHasSeriesLines](./gethasserieslines/) | 如果堆积柱形图或条形图具有系列线，或如果饼图中的饼图或条形图中的饼图在两个部分之间有连接线，则为 True。仅适用于堆积柱形图、条形图、饼图中的饼图或条形图中的饼图。 |
| [SetHasSeriesLines](./sethasserieslines/) | 如果堆积柱形图或条形图具有系列线，或如果饼图中的饼图或条形图中的饼图在两个部分之间有连接线，则为 True。仅适用于堆积柱形图、条形图、饼图中的饼图或条形图中的饼图。 |
| [GetSeriesLines](./getserieslines/) | 返回一个 SeriesLines 对象，表示堆积条形图或堆积柱形图的系列线。仅适用于堆积条形图和堆积柱形图。 |
| [GetHasDropLines](./gethasdroplines/) | 如果图表具有下垂线，则为 True。仅适用于折线图或面积图。 |
| [SetHasDropLines](./sethasdroplines/) | 如果图表具有下垂线，则为 True。仅适用于折线图或面积图。 |
| [GetDropLines](./getdroplines/) | 返回一个 Line 对象，表示折线图或面积图中系列的下垂线。仅适用于折线图或面积图。 |
| [GetHasUpDownBars](./gethasupdownbars/) | 如果折线图具有上升和下降柱，则为 True。仅适用于折线图。 |
| [SetHasUpDownBars](./sethasupdownbars/) | 如果折线图具有上升和下降柱，则为 True。仅适用于折线图。 |
| [GetUpBars](./getupbars/) | 返回一个 DropBars 对象，表示折线图上的上升柱。仅适用于折线图。 |
| [GetDownBars](./getdownbars/) | 返回一个 DropBars 对象，表示折线图上的下降柱。仅适用于折线图。 |
| [IsColorVaried](./iscolorvaried/) | 表示点的颜色是否多变。图表必须仅包含一个系列，或该图表为饼图。 |
| [SetIsColorVaried](./setiscolorvaried/) | 表示点的颜色是否多变。图表必须仅包含一个系列，或该图表为饼图。 |
| [GetGapWidth](./getgapwidth/) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [SetGapWidth](./setgapwidth/) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [GetFirstSliceAngle](./getfirstsliceangle/) | 获取或设置第一个饼图或环形图切片的角度，单位为度（从垂直方向顺时针）。仅适用于饼图、3D 饼图和环形图，取值范围为 0 到 360。 |
| [SetFirstSliceAngle](./setfirstsliceangle/) | 获取或设置第一个饼图或环形图切片的角度，单位为度（从垂直方向顺时针）。仅适用于饼图、3D 饼图和环形图，取值范围为 0 到 360。 |
| [GetOverlap](./getoverlap/) | 指定条形和柱形的定位方式。取值范围为 -100 到 100。仅适用于二维条形图和二维柱形图。 |
| [SetOverlap](./setoverlap/) | 指定条形和柱形的定位方式。取值范围为 -100 到 100。仅适用于二维条形图和二维柱形图。 |
| [GetSecondPlotSize](./getsecondplotsize/) | 返回或设置饼图中的饼图或条形图中的饼图的次要部分的大小，作为主饼图大小的百分比。取值范围为 5 到 200。 |
| [SetSecondPlotSize](./setsecondplotsize/) | 返回或设置饼图中的饼图或条形图中的饼图的次要部分的大小，作为主饼图大小的百分比。取值范围为 5 到 200。 |
| [GetSplitType](./getsplittype/) | 返回或设置用于确定哪些数据点位于饼图中的饼图或条形图中的饼图的第二个饼或条的值。 |
| [SetSplitType](./setsplittype/) | 返回或设置用于确定哪些数据点位于饼图中的饼图或条形图中的饼图的第二个饼或条的值。 |
| [GetSplitValue](./getsplitvalue/) | 返回或设置用于确定哪些数据点位于饼图中的饼图或条形图中的饼图的第二个饼或条的值。 |
| [SetSplitValue](./setsplitvalue/) | 返回或设置用于确定哪些数据点位于饼图中的饼图或条形图中的饼图的第二个饼或条的值。 |
| [IsAutoSplit](./isautosplit/) | 指示阈值是否为自动。 |
| [GetBubbleScale](./getbubblescale/) | 获取或设置指定图表组中气泡的比例因子。取值可以是 0（零）到 300 的整数，对应默认大小的百分比。仅适用于气泡图。 |
| [SetBubbleScale](./setbubblescale/) | 获取或设置指定图表组中气泡的比例因子。取值可以是 0（零）到 300 的整数，对应默认大小的百分比。仅适用于气泡图。 |
| [GetSizeRepresents](./getsizerepresents/) | 获取或设置气泡图中气泡大小所代表的含义。 |
| [SetSizeRepresents](./setsizerepresents/) | 获取或设置气泡图中气泡大小所代表的含义。 |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | 如果为图表组显示负气泡，则为 True。仅对气泡图有效。 |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | 如果为图表组显示负气泡，则为 True。仅对气泡图有效。 |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | 返回或设置环形图组中孔的大小。孔的大小以图表尺寸的百分比表示，介于 10% 到 90% 之间。 |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | 返回或设置环形图组中孔的大小。孔的大小以图表尺寸的百分比表示，介于 10% 到 90% 之间。 |
| [GetExplosion](./getexplosion/) | 打开的饼块与饼图中心的距离以饼直径的百分比表示。 |
| [SetExplosion](./setexplosion/) | 打开的饼块与饼图中心的距离以饼直径的百分比表示。 |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | 如果雷达图具有类别轴标签，则为 True。仅适用于雷达图。 |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | 如果雷达图具有类别轴标签，则为 True。仅适用于雷达图。 |
| [GetHasLeaderLines](./gethasleaderlines/) | 如果系列具有引导线，则为 True。 |
| [SetHasLeaderLines](./sethasleaderlines/) | 如果系列具有引导线，则为 True。 |
| [GetLeaderLines](./getleaderlines/) | 表示图表上的引导线。引导线将数据标签连接到数据点。此对象不是集合；没有表示单个引导线的对象。 |
| [GetLegendEntry](./getlegendentry/) | 根据此系列获取图例项。 |
| [GetShapeProperties](./getshapeproperties/) | 获取保存系列可视形状属性的 ShapePropertyCollection 对象。 |
