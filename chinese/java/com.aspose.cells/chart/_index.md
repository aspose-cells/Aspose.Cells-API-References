---
title: "图表"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单个 Excel 图表的对象。"
type: docs
url: /zh/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

封装表示单个 Excel 图表的对象。

**Example**

以下代码演示如何使用 .NET 代码创建图表。

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [calculate()](#calculate--) | 如果绘图区域和坐标轴的位置是自动分配的，则计算它们的自定义位置。 |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | 使用图表计算选项，在绘图区域和坐标轴位置自动分配时，计算它们的自定义位置。 |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | 使用预设模板更改图表类型。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | 获取图表的实际尺寸（单位为像素）。 |
| [getActualSize()](#getActualSize--) | 获取图表的实际尺寸（单位为像素）。 |
| [getAutoScaling()](#getAutoScaling--) | 如果 Microsoft Excel 对 3D 图表进行缩放，使其大小更接近等效的 2D 图表，则为 true。 |
| [getBackWall()](#getBackWall--) | 返回一个 [getWalls()](../../com.aspose.cells/chart\\#getWalls--) 对象，表示 3D 图表的后墙。 |
| [getCategoryAxis()](#getCategoryAxis--) | 获取图表的 X 轴。 |
| [getChartArea()](#getChartArea--) | 获取工作表中的图表区域。 |
| [getChartDataRange()](#getChartDataRange--) | 获取图表的数据源范围。 |
| [getChartDataTable()](#getChartDataTable--) | 表示图表数据表。 |
| [getChartObject()](#getChartObject--) | 表示 chartShape； |
| [getChartShape()](#getChartShape--) | 表示 chartShape； |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | 表示 3D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。 |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | 指示是否将 \\#N/A 显示为空值。 |
| [getElevation()](#getElevation--) | 表示 3D 图表视图的仰角，以度数为单位。 |
| [getFilteredNSeries()](#getFilteredNSeries--) | 获取一个表示在图表中被过滤的数据系列的 [SeriesCollection](../../com.aspose.cells/seriescollection) 集合。 |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | 获取第一个饼图或环形图切片的角度，单位为度（顺时针从垂直方向）。 |
| [getFloor()](#getFloor--) | 返回一个表示三维图表墙面的 [getFloor()](../../com.aspose.cells/chart\\#getFloor--) 对象。 |
| [getGapDepth()](#getGapDepth--) | 获取三维图表中数据系列之间的距离，作为标记宽度的百分比。 |
| [getGapWidth()](#getGapWidth--) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。 |
| [getHeightPercent()](#getHeightPercent--) | 返回或设置三维图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。 |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | 指示是否仅在图表为 PivotChart 时隐藏枢轴图字段按钮。 |
| [getIs3D()](#getIs3D--) | 指示该图表是否为三维图表。 |
| [getLegend()](#getLegend--) | 获取图表图例。 |
| [getLine()](#getLine--) | 获取线条。 |
| [getNSeries()](#getNSeries--) | 获取一个表示图表中数据系列的 [SeriesCollection](../../com.aspose.cells/seriescollection) 集合。 |
| [getName()](#getName--) | 获取图表的名称。 |
| [getPageSetup()](#getPageSetup--) | 表示此图表的页面设置描述。 |
| [getPerspective()](#getPerspective--) | 返回或设置三维图表视图的透视角度。 |
| [getPivotOptions()](#getPivotOptions--) | 指定显示在图表上的枢轴控件。 |
| [getPivotSource()](#getPivotSource--) | 源是枢轴表的数据。 |
| [getPlacement()](#getPlacement--) | 表示图表附着在其下方单元格的方式。 |
| [getPlotArea()](#getPlotArea--) | 获取图表的绘图区域，其中包括坐标轴刻度标签。 |
| [getPlotBy()](#getPlotBy--) | 获取是按行还是按列绘图。 |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | 获取空单元格的绘图方式。 |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | 指示是否仅绘制可见单元格。 |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | 指示是否仅绘制可见单元格。 |
| [getPrintSize()](#getPrintSize--) | 获取打印的图表尺寸。 |
| [getRightAngleAxes()](#getRightAngleAxes--) | 如果图表坐标轴呈直角，则为 true。 |
| [getRotationAngle()](#getRotationAngle--) | 表示三维图表视图的旋转（绘图区域围绕 Z 轴的旋转，单位为度）。 |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | 获取图表的第二 X 轴。 |
| [getSecondValueAxis()](#getSecondValueAxis--) | 获取图表的第二 Y 轴。 |
| [getSeriesAxis()](#getSeriesAxis--) | 获取图表的系列轴。 |
| [getShapes()](#getShapes--) | 返回此图表中的所有绘图形状。 |
| [getShowDataTable()](#getShowDataTable--) | 获取一个值，指示图表是否显示数据表。 |
| [getShowLegend()](#getShowLegend--) | 获取一个值，指示是否显示图表图例。 |
| [getSideWall()](#getSideWall--) | 返回一个 [getWalls()](../../com.aspose.cells/chart\#getWalls--) 对象，表示 3-D 图表的侧墙。 |
| [getSizeWithWindow()](#getSizeWithWindow--) | 如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 True。 |
| [getStyle()](#getStyle--) | 获取内置样式。 |
| [getSubTitle()](#getSubTitle--) | 获取图表的副标题。 |
| [getTitle()](#getTitle--) | 获取图表的标题。 |
| [getType()](#getType--) | 获取图表的类型。 |
| [getValueAxis()](#getValueAxis--) | 获取图表的 Y 轴。 |
| [getWalls()](#getWalls--) | 返回一个 [getWalls()](../../com.aspose.cells/chart\#getWalls--) 对象，表示 3-D 图表的墙体。 |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | 如果在 3-D 图表上以二维方式绘制网格线，则为 True。 |
| [getWorksheet()](#getWorksheet--) | 获取包含此图表的工作表。 |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | 返回图表上存在哪些轴。 |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | 返回图表所引用的单元格。 |
| [isChartDataChanged()](#isChartDataChanged--) | 检测图表的数据源是否已更改。 |
| [isRectangularCornered()](#isRectangularCornered--) | 获取一个值，指示图表区域是否为矩形角。 |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | 返回该单元格是否被图表引用。 |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | 将图表移动到指定位置。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | 从数据透视表刷新图表数据。 |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | 如果 Microsoft Excel 对 3D 图表进行缩放，使其大小更接近等效的 2D 图表，则为 true。 |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | 指定图表的数据范围。 |
| [setDepthPercent(int value)](#setDepthPercent-int-) | 表示 3D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。 |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | 指示是否将 \\#N/A 显示为空值。 |
| [setElevation(int value)](#setElevation-int-) | 表示 3D 图表视图的仰角，以度数为单位。 |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | 设置第一个饼图或环形图切片的角度，单位为度（顺时针从垂直方向起）。 |
| [setGapDepth(int value)](#setGapDepth-int-) | 设置 3-D 图表中数据系列之间的距离，作为标记宽度的百分比。 |
| [setGapWidth(int value)](#setGapWidth-int-) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。 |
| [setHeightPercent(int value)](#setHeightPercent-int-) | 返回或设置三维图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。 |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | 指示是否仅在图表为 PivotChart 时隐藏枢轴图字段按钮。 |
| [setName(String value)](#setName-java.lang.String-) | 设置图表的名称。 |
| [setPerspective(short value)](#setPerspective-short-) | 返回或设置三维图表视图的透视角度。 |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | 源是枢轴表的数据。 |
| [setPlacement(int value)](#setPlacement-int-) | 表示图表附着在其下方单元格的方式。 |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | 设置空单元格的绘制方式。 |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | 指示是否仅绘制可见单元格。 |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | 指示是否仅绘制可见单元格。 |
| [setPrintSize(int value)](#setPrintSize-int-) | 设置打印图表的尺寸。 |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | 设置一个值，指示图表区域是否为矩形角。 |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | 如果图表坐标轴呈直角，则为 true。 |
| [setRotationAngle(int value)](#setRotationAngle-int-) | 表示三维图表视图的旋转（绘图区域围绕 Z 轴的旋转，单位为度）。 |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | 设置一个值，指示图表是否显示数据表。 |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | 设置一个值，指示是否显示图例。 |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | 如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 True。 |
| [setStyle(int value)](#setStyle-int-) | 设置内置样式。 |
| [setType(int value)](#setType-int-) | 设置图表的类型。 |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | 如果在 3-D 图表上以二维方式绘制网格线，则为 True。 |
| [switchRowColumn()](#switchRowColumn--) | 切换行/列。 |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | 创建图表图像并以指定格式保存到流中。 |
| [toImage(String imageFile)](#toImage-java.lang.String-) | 创建图表图像并保存到文件。 |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | 创建图表图像并以指定格式保存到文件。 |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | 创建图表图像并保存到文件。 |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | 创建图表图像并以指定的图像类型保存到文件。 |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | 创建图表图像并以 JPEG 格式保存到文件。 |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | 创建图表 PDF 并保存到流中。 |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | 创建图表 PDF 并保存到流中。 |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | 将图表保存为 PDF 文件。 |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | 将图表保存为 PDF 文件。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


如果绘图区域和坐标轴的位置是自动分配的，则计算它们的自定义位置。

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


使用图表计算选项，在绘图区域和坐标轴位置自动分配时，计算它们的自定义位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


使用预设模板更改图表类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数据 | byte[] | 图表模板文件（.crtx）的数据。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


获取图表的实际尺寸（单位为像素）。

**Remarks**

注意：此成员已过时。请改用 Chart.getActualSize() 方法。此属性将在自 2022 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int[] - 实际尺寸的数组（宽度和高度）。[0] 为宽度；[1] 为高度。
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


获取图表的实际尺寸（单位为像素）。

**Returns:**
int[] - 实际尺寸的数组（宽度和高度）。[0] 为宽度；[1] 为高度。
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


如果 Microsoft Excel 对 3-D 图表进行缩放，使其尺寸更接近等效的 2-D 图表，则为 True。RightAngleAxes 属性必须为 True。

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


返回一个 [getWalls()](../../com.aspose.cells/chart\\#getWalls--) 对象，表示 3D 图表的后墙。

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


获取图表的 X 轴。

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


获取工作表中的图表区域。

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


获取图表的数据源范围。

**Remarks**

仅支持范围。如果 Series.Values、Name 和 XValues 位于连续范围内，则返回包含它们的范围。

**Returns:**
java.lang.String - 数据源。
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


表示图表数据表。

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


表示 chartShape；

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


表示 chartShape；

**Remarks**

注意：此成员已过时。请改用 Aspose.Cells.Charts.Chart.ChartObject 属性。此属性将在自 2012 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


表示 3D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


指示是否将 \\#N/A 显示为空值。

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


表示 3D 图表视图的仰角，以度数为单位。

**Remarks**

图表仰角是您观看图表的高度，以度为单位。大多数图表类型的默认值为 15。此属性的值必须在 -90 到 90 之间，除 3-D 条形图外，后者必须在 0 到 44 之间。

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


获取一个表示在图表中被过滤的数据系列的 [SeriesCollection](../../com.aspose.cells/seriescollection) 集合。

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


获取第一块饼图或环形图切片的角度，以度为单位（从垂直方向顺时针）。仅适用于饼图、3-D 饼图和环形图，范围为 0 到 360。

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


返回一个表示三维图表墙面的 [getFloor()](../../com.aspose.cells/chart\\#getFloor--) 对象。

**Remarks**

此属性不适用于 3-D 饼图。

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


获取 3-D 图表中数据系列之间的距离，以标记宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


返回或设置条形或柱形簇之间的间距，以条形或柱形宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


返回或设置三维图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


指示是否仅在图表为 PivotChart 时隐藏枢轴图字段按钮。

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


指示该图表是否为三维图表。

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


获取图表图例。

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


获取线条。

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


获取一个表示图表中数据系列的 [SeriesCollection](../../com.aspose.cells/seriescollection) 集合。

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


获取图表的名称。

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


表示此图表的页面设置描述。

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


返回或设置三维图表视图的透视。必须在 0 到 100 之间。如果 RightAngleAxes 属性为 True，则此属性被忽略。

**Returns:**
短
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


指定显示在图表上的枢轴控件。

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


源是透视表的数据。如果 PivotSource 不为空，则该图表为透视图表。

**Remarks**

如果在文件 "Book1.xls" 的工作表 "Sheet1" 中有透视表 "PivotTable1"。如果图表和透视表不在同一工作簿中，pivotSource 可以是 "[Book1.xls]Sheet1!PivotTable1"。如果设置此属性，之前的数据源设置将丢失。

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


表示图表附着在其下方单元格的方式。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


获取图表的绘图区域，其中包括坐标轴刻度标签。

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


获取是按行还是按列绘图。

参见 [PlotDataByType](../../com.aspose.cells/plotdatabytype)。

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


获取空单元格的绘图方式。

参见 [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype)。

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


指示是否仅绘制可见单元格。

**Remarks**

注意：此成员已过时。请改用 PlotVisibleCellsOnly 属性。此方法将在自 2022 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


指示是否仅绘制可见单元格。

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


获取打印的图表尺寸。

参见 [PrintSizeType](../../com.aspose.cells/printsizetype)。

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


如果图表坐标轴呈直角则为 True。仅适用于 3-D 图表（除 Column3D 和 3-D 饼图外）。

**Remarks**

如果此属性为 True，则忽略 Perspective 属性。

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


表示三维图表视图的旋转（绘图区域围绕 Z 轴的旋转，单位为度）。

**Remarks**

此属性的值必须在 0 到 360 之间，除 3-D 条形图外，后者的值必须在 0 到 44 之间。默认值为 20。仅适用于 3-D 图表。

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


获取图表的第二 X 轴。

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


获取图表的第二 Y 轴。

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


获取图表的系列轴。

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


返回此图表中的所有绘图形状。

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


获取一个值，指示图表是否显示数据表。

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


获取一个值，指示是否显示图例。默认值为 true。

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


返回一个 [getWalls()](../../com.aspose.cells/chart\#getWalls--) 对象，表示 3-D 图表的侧墙。

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 True。

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


获取内置样式。

**Remarks**

应在 1 到 48 之间。如果未设置则返回 -1。

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


获取图表的副标题。仅适用于 ODS 文件。

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


获取图表的标题。

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


获取图表的类型。

参见 [ChartType](../../com.aspose.cells/charttype)。

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


获取图表的 Y 轴。

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


返回一个 [getWalls()](../../com.aspose.cells/chart\#getWalls--) 对象，表示 3-D 图表的墙体。

**Remarks**

此属性不适用于 3-D 饼图。

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


如果在 3-D 图表上以二维方式绘制网格线，则为 True。

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取包含此图表的工作表。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


返回图表上存在哪些轴。

**Remarks**

通常，Pie、PieExploded、PiePie、PieBar、Pie3D、Pie3DExploded、Doughnut、DoughnutExploded 没有坐标轴。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


返回图表所引用的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 工作表索引。-1 表示包含当前图表的工作表。 |
| rowIndex | int | 行索引 |
| columnIndex | int | 列索引 |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


检测图表的数据源是否已更改。

**Remarks**

该方法在将图表渲染为图像格式之前检测图表数据源的更改。首次调用 Chart.toImage 时，图表源数据（例如 XValuesParseData、ValuesParseData）将被记录。在再次调用 Chart.toImage 方法之前，调用 IsChartDataChanged 方法检查图表是否需要重新渲染。

**Returns:**
boolean - 如果图表已更改则返回 true，否则返回 false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


获取一个值，指示图表区域是否为矩形角。默认值为 true。

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


返回该单元格是否被图表引用。

**Remarks**

注意：此方法现已过时。请改用 IsCellReferedByChart(int,int,int) 方法。该方法将在自 2023 年 4 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引 |
| columnIndex | int | 列索引 |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


将图表移动到指定位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


从数据透视表刷新图表数据。

**Remarks**

我们将从透视数据源收集数据到透视表报告。此方法仅用于将所有数据收集到透视图表中。

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


如果 Microsoft Excel 对 3-D 图表进行缩放，使其尺寸更接近等效的 2-D 图表，则为 True。RightAngleAxes 属性必须为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


指定图表的数据范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | java.lang.String | 指定用于绘制数据系列的值 |
| isVertical | boolean | 指定是按行还是按列从单元格值范围绘制系列。 |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


表示 3D 图表的深度，作为图表宽度的百分比（介于 20% 到 2000% 之间）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


指示是否将 \\#N/A 显示为空值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


表示 3D 图表视图的仰角，以度数为单位。

**Remarks**

图表仰角是您观看图表的高度，以度为单位。大多数图表类型的默认值为 15。此属性的值必须在 -90 到 90 之间，除 3-D 条形图外，后者必须在 0 到 44 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


设置第一块饼图或环形图切片的角度，单位为度（从垂直方向顺时针）。仅适用于饼图、3D 饼图和环形图，范围为 0 到 360。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


设置 3D 图表中数据系列之间的距离，以标记宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


返回或设置条形或柱形簇之间的间距，以条形或柱形宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


返回或设置三维图表的高度，作为图表宽度的百分比（介于 5% 到 500% 之间）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


指示是否仅在图表为 PivotChart 时隐藏枢轴图字段按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置图表的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


返回或设置三维图表视图的透视。必须在 0 到 100 之间。如果 RightAngleAxes 属性为 True，则此属性被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


源是透视表的数据。如果 PivotSource 不为空，则该图表为透视图表。

**Remarks**

如果在文件 "Book1.xls" 的工作表 "Sheet1" 中有透视表 "PivotTable1"。如果图表和透视表不在同一工作簿中，pivotSource 可以是 "[Book1.xls]Sheet1!PivotTable1"。如果设置此属性，之前的数据源设置将丢失。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


表示图表附着在其下方单元格的方式。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


设置空单元格的绘制方式。

参见 [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


指示是否仅绘制可见单元格。

**Remarks**

注意：此成员已过时。请改用 PlotVisibleCellsOnly 属性。此方法将在自 2022 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


指示是否仅绘制可见单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


设置打印图表的尺寸。

参见 [PrintSizeType](../../com.aspose.cells/printsizetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


设置一个值，指示图表区域是否为矩形角。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


如果图表坐标轴呈直角则为 True。仅适用于 3-D 图表（除 Column3D 和 3-D 饼图外）。

**Remarks**

如果此属性为 True，则忽略 Perspective 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


表示三维图表视图的旋转（绘图区域围绕 Z 轴的旋转，单位为度）。

**Remarks**

此属性的值必须在 0 到 360 之间，除 3-D 条形图外，后者的值必须在 0 到 44 之间。默认值为 20。仅适用于 3-D 图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


设置一个值，指示图表是否显示数据表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


设置一个值，指示是否显示图例。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


如果 Microsoft Excel 将图表大小调整为匹配图表工作表窗口的大小，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


设置内置样式。

**Remarks**

应在 1 到 48 之间。如果未设置则返回 -1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置图表的类型。

参见 [ChartType](../../com.aspose.cells/charttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


如果在 3-D 图表上以二维方式绘制网格线，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


切换行/列。

**Returns:**
boolean - False 表示切换行/列失败。
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


创建图表图像并以指定格式保存到流中。

**Remarks**

图像的格式通过使用 `options.ImageFormat` 指定。支持以下格式：ImageFormat.Bmp、ImageFormat.Gif、ImageFormat.Png、ImageFormat.Jpeg、ImageFormat.Tiff、ImageFormat.Emf。

如果宽度或高度为零，或根据 Supported Charts List 不支持该图表，则此方法不执行任何操作。详情请参阅 [Supported Charts List][]。


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 输出流。 |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 附加图像创建选项 |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


创建图表图像并将其保存到文件。文件名的扩展名决定图像的格式。

**Remarks**

图像的格式通过使用文件名的扩展名指定。例如，如果指定 \"myfile.png\"，则图像将以 PNG 格式保存。支持以下文件扩展名：.bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。

如果宽度或高度为零，或根据 Supported Charts List 不支持该图表，则此方法不执行任何操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String | 包含完整路径的图像文件名。 |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


创建图表图像并以指定格式保存到文件。

**Remarks**

注意：此成员现已过时。请改用 Chart.ToImage(string, ImageType) 方法。该属性将在自 2022 年 7 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String | 包含完整路径的图像文件名。 |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | 保存图像的格式。 |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


创建图表图像并将其保存到文件。文件名的扩展名决定图像的格式。

**Remarks**

图像的格式通过使用文件名的扩展名指定。例如，如果指定 \"myfile.png\"，则图像将以 PNG 格式保存。支持以下文件扩展名：.bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。

如果宽度或高度为零，或根据 Supported Charts List 不支持该图表，则此方法不执行任何操作。详情请参阅 [Supported Charts List][]。

**Example**

以 300 dpi 和 CCITT4 压缩保存为 Tiff。

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String | 包含完整路径的图像文件名。 |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 附加图像创建选项 |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


创建图表图像并以指定的图像类型保存到文件。

**Remarks**

图像的类型通过使用 `imageType` 指定。支持以下类型：ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。

如果宽度或高度为零，或根据 Supported Charts List 不支持该图表，则此方法不执行任何操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String | 包含完整路径的图像文件名。 |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype)。用于保存图像的图像类型。 |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


创建图表图像并以 JPEG 格式保存到文件。

**Remarks**

如果宽度或高度为零，或根据 Supported Charts List 不支持该图表，则此方法不执行任何操作。注意：此方法现已过时。请改用带有指定质量的 ToImage(string,ImageOrPrintOptions) 方法。该方法将在自 2025 年 3 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String | 包含完整路径的图像文件名。 |
| jpegQuality | long | Jpeg 质量。 |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


创建图表 PDF 并保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 输出流。 |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


创建图表 PDF 并保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 输出流。 |
| desiredPageWidth | float | 所需的页面宽度（英寸）。 |
| desiredPageHeight | float | 所需的页面高度（英寸）。 |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). 输出页面中图表的水平对齐类型。 |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). 输出页面中图表的垂直对齐类型。 |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


将图表保存为 PDF 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | PDF 文件的完整路径名称 |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


将图表保存为 PDF 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | PDF 文件的完整路径名称 |
| desiredPageWidth | float | 所需的页面宽度（英寸）。 |
| desiredPageHeight | float | 所需的页面高度（英寸）。 |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). 输出页面中图表的水平对齐类型。 |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). 输出页面中图表的垂直对齐类型。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

