---
title: Chart
second_title: Aspose.Cells for .NET API 参考
description: 封装表示单个 Excel 图表的对象
type: docs
weight: 430
url: /zh/net/aspose.cells.charts/chart/
---
## Chart class

封装表示单个 Excel 图表的对象。

```csharp
public class Chart
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | 如果 Microsoft Excel 缩放 3-D 图表以使其尺寸更接近等效的 2-D 图表，则为真。 RightAngleAxes 属性必须为 True。 |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | 返回一个[`Walls`](./walls)对象，该对象表示 3-D 图表的后墙。 |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | 获取图表的 X 轴。 |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | 获取工作表中的图表区域。 |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | 表示图表数据表。 |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | 表示图表形状； |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | 将 3-D 图表的深度表示为图表宽度的百分比（介于 20% 和 2000% 之间）。 |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | 指示是否将#N/A 显示为空白值。 |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | 表示 3-D 图表视图的高度，以度为单位。 |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | 获取或设置第一个饼图或圆环图切片的角度，以度为单位（从垂直顺时针方向）。仅适用于饼图、3-D 饼图和圆环图，0 到 360。 |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | 返回一个[`Floor`](./floor)对象，该对象表示 3-D 图表的墙壁。 |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | 获取或设置 3-D 图表中数据系列之间的距离，以标记宽度的百分比表示。 该属性的值必须介于 0 和 500 之间。 |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | 返回或设置条形或列簇之间的间距，以条形或列宽的百分比表示。 该属性的值必须介于 0 和 500 之间。 |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | 返回或设置 3-D 图表的高度为图表宽度的百分比（介于 5% 和 500% 之间）。 |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | 表示是否仅在图表为数据透视图时隐藏数据透视图字段按钮。 |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | 表示图表是否为 3d 图表。 |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | 获取或设置一个值，指示图表区域是否为矩形角。 默认为真。 |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | 获取图表图例。 |
| [Line](../../aspose.cells.charts/chart/line) { get; } | 获取线路。 |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | 获取和设置图表的名称。 |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | 获取表示图表中数据系列的[`SeriesCollection`](../seriescollection)集合。 |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | 表示此图表中的页面设置说明。 |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | 返回或设置 3-D 图表视图的透视图。必须介于 0 和 100 之间。 如果 RightAngleAxes 属性为 True，则忽略此属性。 |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | 指定图表上出现的枢轴控件 |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | 来源是pivotTable的数据。 如果 PivotSource 不为空，则图表为 PivotChart。 |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | 表示图表附加到其下方单元格的方式。 |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | 获取图表的绘图区域，其中包括轴刻度标签。 |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | 获取和设置是按行还是按列绘制。 |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | 获取并设置如何绘制空单元格。 |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | 表示是否只绘制可见单元格。 |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | 获取和设置打印的图表大小。 |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | 如果图表轴成直角，则为真。仅适用于 3-D 图表（Column3D 和 3-D 饼图除外）。 |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | 表示 3-D 图表视图的旋转（绘图区域围绕 z 轴的旋转，以度为单位）。 |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | 获取图表的第二个 X 轴。 |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | 获取图表的第二个 Y 轴。 |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | 获取图表的系列轴。 |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | 返回此图表中的所有绘图形状。 |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | 获取或设置图表是否显示数据表的值。 |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | 获取或设置是否显示图表图例的值。默认为真。 |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | 返回代表 3-D 图表侧壁的[`Walls`](./walls)对象。 |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | 如果 Microsoft Excel 调整图表大小以匹配图表工作表窗口的大小，则为真。 |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | 获取和设置内置样式。 |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | 获取图表的副标题。 仅适用于 ODS 格式文件。 |
| [Title](../../aspose.cells.charts/chart/title) { get; } | 获取图表的标题。 |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | 获取或设置图表的类型。 |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | 获取图表的 Y 轴。 |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | 返回一个[`Walls`](./walls)对象，表示 3-D 图表的墙壁。 |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | 如果网格线在 3-D 图表上以二维方式绘制，则为真。 |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | 获取包含此图表的工作表。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | 计算绘图区域的自定义位置，如果坐标轴的位置是自动分配的。 |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | 以像素为单位获取图表的实际大小。 |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | 获取图表的数据源范围。 |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | 返回图表上存在哪些轴。 |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | 检测图表的数据源是否已更改。 |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | 将图表移动到指定位置。 |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | 从它的透视数据源刷新透视图的数据。 |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | 指定图表的数据范围。 |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | 切换行/列。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | 获取图表的 32 位` 位图` 对象。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | 获取图表的 32 位` 位图` 对象。 ` ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression 和 ImageOrPrintOptions.Quality 属性被忽略。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_5)(string) | 创建图表图像并将其保存到文件中。 文件名的扩展名决定了图像的格式。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, ImageFormat) | 创建图表图像并将其保存到指定格式的流中。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageOrPrintOptions) | 创建图表图像并将其保存到指定格式的流中。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, long) | 创建图表图像并将其保存到 Jpeg 格式的流中。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageFormat) | 创建图表图像并将其保存到指定格式的文件中。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string, ImageOrPrintOptions) | 创建图表图像并将其保存到文件中。 文件名的扩展名决定了图像的格式。 |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, long) | 创建图表图像并将其保存到 Jpeg 格式的文件中。 |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | 创建图表 pdf 并将其保存到流中。 |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | 将图表保存为 pdf 文件。 |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | 创建图表 pdf 并将其保存到流中。 |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | 将图表保存为 pdf 文件。 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### 也可以看看

* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
