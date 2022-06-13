---
title: Aspose.Cells.Charts
second_title: Aspose.Cells for .NET API 参考
description: 包含所有类的图表和迷你图
type: docs
weight: 20
url: /zh/net/aspose.cells.charts/
---
包含所有类的图表和迷你图。

## 课程

| 班级 | 描述 |
| --- | --- |
| [Axis](./axis) | 封装表示图表轴的对象。 |
| [AxisBins](./axisbins) | 表示轴箱 |
| [Chart](./chart) | 封装表示单个 Excel 图表的对象。 |
| [ChartArea](./chartarea) | 封装表示工作表中图表区域的对象。 |
| [ChartCollection](./chartcollection) | 封装[`Chart`](../aspose.cells.charts/chart)对象的集合。 |
| [ChartDataTable](./chartdatatable) | 表示图表数据表。 |
| [ChartFrame](./chartframe) | 在图表中封装表示框架对象的对象。 |
| [ChartGlobalizationSettings](./chartglobalizationsettings) | 表示图表的全球化设置。 |
| [ChartPoint](./chartpoint) | 表示图表中系列中的单个点。 |
| [ChartPointCollection](./chartpointcollection) | 表示包含一个系列中所有点的集合。 |
| [ChartTextFrame](./charttextframe) | 封装表示包含文本的框架对象的对象。 |
| [DataLabels](./datalabels) | 封装指定系列的所有 DataLabel 对象的集合。 |
| [DisplayUnitLabel](./displayunitlabel) | 表示显示单元标签。 |
| [DropBars](./dropbars) | 表示图表中的向上/向下柱。 |
| [ErrorBar](./errorbar) | 代表数据系列的误差线。 |
| [Floor](./floor) | 封装表示 3-D 图表地板的对象。 |
| [Legend](./legend) | 封装表示图表图例的对象。 |
| [LegendEntry](./legendentry) | 表示图表图例中的图例条目。 |
| [LegendEntryCollection](./legendentrycollection) | 表示指定图表图例中所有[`LegendEntry`](../aspose.cells.charts/legendentry)对象的集合。 |
| [Marker](./marker) | 表示折线图、散点图或雷达图中的标记。 |
| [PivotOptions](./pivotoptions) | 表示复杂类型，指定出现在图表上的枢轴控件 |
| [PlotArea](./plotarea) | 封装表示图表中绘图区域的对象。 |
| [Series](./series) | 封装表示图表中单个数据系列的对象。 |
| [SeriesCollection](./seriescollection) | 封装[`Series`](../aspose.cells.charts/series)对象的集合。 |
| [SeriesLayoutProperties](./serieslayoutproperties) |  |
| [Sparkline](./sparkline) | 迷你图表示工作表单元格中的小图表或图形，提供数据的可视化表示。  &lt;code&gt; [C#] Workbook book = new Workbook(); 工作表工作表 = book.Worksheets[0]; sheet.Cells["A1"].PutValue(5); sheet.Cells["B1"].PutValue(2); sheet.Cells["C1"].PutValue(1); sheet.Cells["D1"].PutValue(3); // 定义 CellArea CellArea ca = new CellArea(); ca.StartColumn = 4; ca.EndColumn = 4; ca.StartRow = 0; ca.EndRow = 0; int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, sheet.Name + "!A1:D1", false, ca); SparklineGroup 组 = sheet.SparklineGroupCollection[idx]; idx = group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4); 迷你图线 = group.SparklineCollection[idx]; Console.WriteLine($"Saprkline 数据范围:{line.DataRange}，行:{line.Row}，列:{line.Column}"); line.ToImage("output.png", new ImageOrPrintOptions()); &lt;/code&gt; |
| [SparklineCollection](./sparklinecollection) | 封装[`Sparkline`](../aspose.cells.charts/sparkline)对象的集合。 |
| [SparklineGroup](./sparklinegroup) | [`Sparkline`](../aspose.cells.charts/sparkline)被组织成迷你图组。 SparklineGroup 包含可变数量的迷你图项目。 迷你图组指定迷你图的类型、显示设置和轴设置。 |
| [SparklineGroupCollection](./sparklinegroupcollection) | 封装[`SparklineGroup`](../aspose.cells.charts/sparklinegroup)对象的集合。 |
| [TickLabelItem](./ticklabelitem) | 包含Ticklabel项的信息 |
| [TickLabels](./ticklabels) | 表示与图表轴上的刻度线相关的刻度线标签。 |
| [Title](./title) | 封装表示图表或轴标题的对象。 |
| [Trendline](./trendline) | 表示图表中的趋势线。 |
| [TrendlineCollection](./trendlinecollection) | 表示指定数据系列的所有[`Trendline`](../aspose.cells.charts/trendline)对象的集合。 |
| [Walls](./walls) | 封装表示 3-D 图表墙壁的对象。 |
## 枚举

| 枚举 | 描述 |
| --- | --- |
| [AxisType](./axistype) | 表示轴类型。 |
| [BackgroundMode](./backgroundmode) | 表示背景的显示方式。 |
| [Bar3DShapeType](./bar3dshapetype) | 表示与 3-D 条形图或柱形图一起使用的形状。 |
| [BubbleSizeRepresents](./bubblesizerepresents) | 代表气泡图上的气泡大小。 |
| [CategoryType](./categorytype) | 表示类别轴类型。 |
| [ChartLineFormattingType](./chartlineformattingtype) | 表示图表线条的线条格式类型。 |
| [ChartMarkerType](./chartmarkertype) | 表示折线图、散点图或雷达图中的标记样式。 |
| [ChartSplitType](./chartsplittype) | 表示饼图或饼图的两个部分的拆分方式。 |
| [ChartTextDirectionType](./charttextdirectiontype) | 表示图表的文字方向类型。 |
| [ChartType](./charttype) | 枚举 Excel 中使用的所有图表类型。 |
| [CrossType](./crosstype) | 表示轴交叉类型。 |
| [DataLabelsSeparatorType](./datalabelsseparatortype) | 表示DataLabels的分隔符类型。 |
| [DisplayUnitType](./displayunittype) | 表示显示单元的类型。 |
| [ErrorBarDisplayType](./errorbardisplaytype) | 代表错误栏显示类型。 |
| [ErrorBarType](./errorbartype) | 表示误差条数量类型。 |
| [FormattingType](./formattingtype) | 表示应用于[`Area`](../aspose.cells.drawing/area)对象或Line对象。 |
| [LabelPositionType](./labelpositiontype) | 表示数据标签位置类型。 |
| [LegendPositionType](./legendpositiontype) | 枚举图例位置类型。 |
| [MapChartLabelLayout](./mapchartlabellayout) | 表示地图标签的布局。 |
| [MapChartProjectionType](./mapchartprojectiontype) | 表示地图的投影类型。 |
| [MapChartRegionType](./mapchartregiontype) | 表示地图的区域类型。 |
| [PlotDataByType](./plotdatabytype) | 表示按行或按列绘制的数据类型。 |
| [PlotEmptyCellsType](./plotemptycellstype) | 表示图表的所有绘图空单元格类型。 |
| [QuartileCalculationType](./quartilecalculationtype) | 表示四分位数计算方法。 |
| [SparklineAxisMinMaxType](./sparklineaxisminmaxtype) | 表示迷你图垂直轴的最小值和最大值类型。 |
| [SparklinePresetStyleType](./sparklinepresetstyletype) | 代表迷你图的预设样式类型。 |
| [SparklineType](./sparklinetype) | 表示迷你图类型。 |
| [TickLabelPositionType](./ticklabelpositiontype) | 表示指定轴上刻度线标签的位置类型。 |
| [TickMarkType](./tickmarktype) | 表示指定轴的刻度线类型。 |
| [TimeUnit](./timeunit) | 表示类别轴的基本单位。 |
| [TrendlineType](./trendlinetype) | 表示趋势线类型。 |

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
