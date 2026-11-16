---
title: "Chart 类"
linktitle: "Chart"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Chart 类。封装了在 Go 中表示 chart 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/chart/
---

## Chart class

封装表示单个 Excel 图表的对象。

```go

type Chart struct  {
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
| [GetStyle](./getstyle/) | 获取和设置内置样式。 |
| [SetStyle](./setstyle/) | 获取和设置内置样式。 |
| [GetChartObject](./getchartobject/) | 表示 chartShape； |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | 指示是否仅在图表为 PivotChart 时隐藏透视图表字段按钮。 |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | 指示是否仅在图表为 PivotChart 时隐藏透视图表字段按钮。 |
| [GetPivotOptions](./getpivotoptions/) | 指定出现在图表上的透视控件 |
| [GetPivotSource](./getpivotsource/) | 源是透视表的数据。如果 PivotSource 不为空，则该图表为 PivotChart。 |
| [SetPivotSource](./setpivotsource/) | 源是透视表的数据。如果 PivotSource 不为空，则该图表为 PivotChart。 |
| [IsCellReferedByChart](./iscellreferedbychart/) | 返回图表所引用的单元格。 |
| [IsChartDataChanged](./ischartdatachanged/) | 检测图表的数据源是否已更改。 |
| [GetPlotBy](./getplotby/) | 获取和设置是按行还是按列绘制。 |
| [RefreshPivotData](./refreshpivotdata/) | 从透视表刷新图表的数据。 |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | 获取和设置空单元格的绘制方式。 |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | 获取和设置空单元格的绘制方式。 |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | 指示是否仅绘制可见单元格。 |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | 指示是否仅绘制可见单元格。 |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | 指示是否将 #N/A 显示为空值。 |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | 指示是否将 #N/A 显示为空值。 |
| [GetName](./getname/) | 获取和设置图表的名称。 |
| [SetName](./setname/) | 获取和设置图表的名称。 |
| [GetSizeWithWindow](./getsizewithwindow/) | 如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 true。 |
| [SetSizeWithWindow](./setsizewithwindow/) | 如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 true。 |
| [GetWorksheet](./getworksheet/) | 获取包含此图表的工作表。 |
| [GetShapes](./getshapes/) | 返回此图表中的所有绘图形状。 |
| [GetPrintSize](./getprintsize/) | 获取和设置打印的图表尺寸。 |
| [SetPrintSize](./setprintsize/) | 获取和设置打印的图表尺寸。 |
| [ChangeTemplate](./changetemplate/) | 使用预设模板更改图表类型。 |
| [GetType](./gettype/) | 获取或设置图表的类型。 |
| [SetType](./settype/) | 获取或设置图表的类型。 |
| [Move](./move/) | 将图表移动到指定位置。 |
| [GetNSeries](./getnseries/) | 获取表示图表中数据系列的 SeriesCollection 集合。 |
| [GetFilteredNSeries](./getfilterednseries/) | 获取表示图表中已过滤数据系列的 SeriesCollection 集合。 |
| [GetTitle](./gettitle/) | 获取图表的标题。 |
| [GetSubTitle](./getsubtitle/) | 获取图表的副标题。仅适用于 ODS 文件。 |
| [GetPlotArea](./getplotarea/) | 获取图表的绘图区，其中包括坐标轴刻度标签。 |
| [GetChartArea](./getchartarea/) | 获取工作表中的图表区域。 |
| [GetCategoryAxis](./getcategoryaxis/) | 获取图表的 X 轴。 |
| [GetValueAxis](./getvalueaxis/) | 获取图表的 Y 轴。 |
| [GetSecondValueAxis](./getsecondvalueaxis/) | 获取图表的第二 Y 轴。 |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | 获取图表的第二 X 轴。 |
| [GetSeriesAxis](./getseriesaxis/) | 获取图表的系列轴。 |
| [GetLegend](./getlegend/) | 获取图表图例。 |
| [GetChartDataTable](./getchartdatatable/) | 表示图表数据表。 |
| [GetShowLegend](./getshowlegend/) | 获取或设置指示是否显示图表图例的值。默认值为 true。 |
| [SetShowLegend](./setshowlegend/) | 获取或设置指示是否显示图表图例的值。默认值为 true。 |
| [IsRectangularCornered](./isrectangularcornered/) | 获取或设置指示图表区域是否为矩形角的值。默认值为 true。 |
| [SetIsRectangularCornered](./setisrectangularcornered/) | 获取或设置指示图表区域是否为矩形角的值。默认值为 true。 |
| [GetShowDataTable](./getshowdatatable/) | 获取或设置指示图表是否显示数据表的值。 |
| [SetShowDataTable](./setshowdatatable/) | 获取或设置指示图表是否显示数据表的值。 |
| [GetFirstSliceAngle](./getfirstsliceangle/) | 获取或设置第一个饼图或环形图切片的角度（以度为单位，顺时针从垂直方向起算）。仅适用于饼图、3D 饼图和环形图，范围 0 到 360。 |
| [SetFirstSliceAngle](./setfirstsliceangle/) | 获取或设置第一个饼图或环形图切片的角度（以度为单位，顺时针从垂直方向起算）。仅适用于饼图、3D 饼图和环形图，范围 0 到 360。 |
| [GetGapWidth](./getgapwidth/) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [SetGapWidth](./setgapwidth/) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [GetGapDepth](./getgapdepth/) | 获取或设置 3D 图表中数据系列之间的距离，作为标记宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [SetGapDepth](./setgapdepth/) | 获取或设置 3D 图表中数据系列之间的距离，作为标记宽度的百分比。此属性的值必须在 0 到 500 之间。 |
| [Calculate](./calculate/) | 如果绘图区和坐标轴的位置是自动分配的，则计算它们的自定义位置。 |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | 使用图表计算选项计算绘图区和坐标轴的自定义位置（如果它们的位置是自动分配的）。 |
| [GetFloor](./getfloor/) | 返回一个 Floor 对象，表示 3-D 图表的墙体。 |
| [GetWalls](./getwalls/) | 返回一个 Walls 对象，表示 3-D 图表的墙体。 |
| [GetBackWall](./getbackwall/) | 返回一个 Walls 对象，表示 3-D 图表的后墙。 |
| [GetSideWall](./getsidewall/) | 返回一个 Walls 对象，表示 3-D 图表的侧墙。 |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | 如果在 3-D 图表上以二维方式绘制网格线，则为 True。 |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | 如果在 3-D 图表上以二维方式绘制网格线，则为 True。 |
| [GetRotationAngle](./getrotationangle/) | 表示 3-D 图表视图的旋转（绘图区绕 Z 轴的旋转，以度为单位）。 |
| [SetRotationAngle](./setrotationangle/) | 表示 3-D 图表视图的旋转（绘图区绕 Z 轴的旋转，以度为单位）。 |
| [GetElevation](./getelevation/) | 表示 3-D 图表视图的仰角，以度为单位。 |
| [SetElevation](./setelevation/) | 表示 3-D 图表视图的仰角，以度为单位。 |
| [GetRightAngleAxes](./getrightangleaxes/) | 如果图表坐标轴呈直角，则为 True。仅适用于 3-D 图表（Column3D 和 3-D 饼图除外）。 |
| [SetRightAngleAxes](./setrightangleaxes/) | 如果图表坐标轴呈直角，则为 True。仅适用于 3-D 图表（Column3D 和 3-D 饼图除外）。 |
| [GetAutoScaling](./getautoscaling/) | 如果 Microsoft Excel 对 3-D 图表进行缩放，使其尺寸更接近等效的 2-D 图表，则为 True。RightAngleAxes 属性必须为 True。 |
| [SetAutoScaling](./setautoscaling/) | 如果 Microsoft Excel 对 3-D 图表进行缩放，使其尺寸更接近等效的 2-D 图表，则为 True。RightAngleAxes 属性必须为 True。 |
| [GetHeightPercent](./getheightpercent/) | 返回或设置 3-D 图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。 |
| [SetHeightPercent](./setheightpercent/) | 返回或设置 3-D 图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。 |
| [GetPerspective](./getperspective/) | 返回或设置三维图表视图的透视度，必须在 0 到 100 之间。如果 RightAngleAxes 属性为 True，则此属性被忽略。 |
| [SetPerspective](./setperspective/) | 返回或设置三维图表视图的透视度，必须在 0 到 100 之间。如果 RightAngleAxes 属性为 True，则此属性被忽略。 |
| [GetIs3D](./getis3d/) | 指示该图表是否为 3d 图表。 |
| [GetDepthPercent](./getdepthpercent/) | 表示 3-D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。 |
| [SetDepthPercent](./setdepthpercent/) | 表示 3-D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。 |
| [ToImage_String](./toimage_string/) | 创建图表图像并将其保存到文件。文件名的扩展名决定图像的格式。 |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | 创建图表图像并以指定的图像类型保存到文件。 |
| [ToImage_Int64](./toimage_int64/) | 创建图表图像并以 Jpeg 格式保存到流中。 |
| [ToImage_ImageType](./toimage_imagetype/) | 创建图表图像并以指定的格式保存到流中。 |
| [ToPdf_String](./topdf_string/) | 将图表保存为 pdf 文件。 |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | 将图表保存为 pdf 文件。 |
| [ToPdf](./topdf/) | 创建图表 PDF 并保存到流中。 |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | 创建图表 pdf 并保存到流中。 |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | 创建图表图像并将其保存到文件。文件名的扩展名决定图像的格式。 |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | 创建图表图像并以指定的格式保存到流中。 |
| [GetActualSize](./getactualsize/) | 获取图表的实际尺寸（单位：像素）。 |
| [GetPlacement](./getplacement/) | 表示图表附着在其下方单元格的方式。 |
| [SetPlacement](./setplacement/) | 表示图表附着在其下方单元格的方式。 |
| [GetPageSetup](./getpagesetup/) | 表示此图表的页面设置描述。 |
| [HasAxis](./hasaxis/) | 返回图表上存在的坐标轴。 |
| [SwitchRowColumn](./switchrowcolumn/) | 切换行/列。 |
| [GetChartDataRange](./getchartdatarange/) | 获取图表的数据源范围。 |
| [SetChartDataRange](./setchartdatarange/) | 指定图表的数据范围。 |
| [GetLine](./getline/) | 获取该线。 |
