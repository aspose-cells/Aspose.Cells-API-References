---
title: "Series"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示图表中单个数据系列的对象。"
type: docs
url: /zh/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

封装表示图表中单个数据系列的对象。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | 表示 Series 对象的背景区域。 |
| [getBar3DShapeType()](#getBar3DShapeType--) | 获取在 3-D 条形图或柱形图中使用的 3D 形状类型。 |
| [getBorder()](#getBorder--) | 表示 Series 对象的边框。 |
| [getBubbleScale()](#getBubbleScale--) | 获取指定图表组中气泡的比例因子。 |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | 获取气泡图中气泡大小所表示的含义。 |
| [getBubbleSizes()](#getBubbleSizes--) | 获取图表系列的气泡大小值。 |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | 获取系列的缓存类别值 |
| [getCachedValues()](#getCachedValues--) | 获取系列的缓存值 |
| [getCategoryValues()](#getCategoryValues--) | 获取用于在图表中绘制此系列每个点的实际类别值。 |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | 获取数据值的数量。 |
| [getDataLabels()](#getDataLabels--) | 表示指定 ASeries 的 DataLabels 对象。 |
| [getDisplayName()](#getDisplayName--) | 获取在图表中显示的系列名称。 |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | 返回或设置环形图组中孔的大小。 |
| [getDownBars()](#getDownBars--) | 返回一个 [DropBars](../../com.aspose.cells/dropbars) 对象，表示折线图上的下垂柱。 |
| [getDropLines()](#getDropLines--) | 返回一个 [Line](../../com.aspose.cells/line) 对象，表示折线图或面积图中系列的下拉线。 |
| [getExplosion()](#getExplosion--) | 打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。 |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | 获取第一个饼图或环形图切片的角度，单位为度（顺时针从垂直方向）。 |
| [getGapWidth()](#getGapWidth--) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。 |
| [getHas3DEffect()](#getHas3DEffect--) | 如果系列具有三维外观，则为 True。 |
| [getHiLoLines()](#getHiLoLines--) | 返回一个 HiLoLines 对象，表示折线图中系列的高低线。 |
| [getLayoutProperties()](#getLayoutProperties--) | 表示布局的属性。 |
| [getLeaderLines()](#getLeaderLines--) | 表示图表上的引线。 |
| [getLegendEntry()](#getLegendEntry--) | 获取对应此系列的图例项。 |
| [getMarker()](#getMarker--) | 获取 [getMarker()](../../com.aspose.cells/series\#getMarker--)。 |
| [getName()](#getName--) | 获取数据系列的名称。 |
| [getOverlap()](#getOverlap--) | 指定条形和柱形的定位方式。 |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | 指示此系列是否绘制在第二值轴上。 |
| [getPointValues()](#getPointValues--) | 获取用于在图表中绘制此系列每个点的实际值。 |
| [getPoints()](#getPoints--) | 获取图表中系列的点集合。 |
| [getSecondPlotSize()](#getSecondPlotSize--) | 返回或设置饼图中的饼图或条形饼图的次要部分的大小，作为主饼图大小的百分比。 |
| [getSeriesLines()](#getSeriesLines--) | 返回一个 SeriesLines 对象，表示堆叠条形图或堆叠柱形图的系列线。 |
| [getShadow()](#getShadow--) | 如果系列具有阴影，则为 True。 |
| [getShapeProperties()](#getShapeProperties--) | 获取 [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) 对象，该对象保存系列的可视形状属性。 |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | 如果为图表组显示负气泡，则为 True。 |
| [getSizeRepresents()](#getSizeRepresents--) | 获取气泡图中气泡大小所表示的含义。 |
| [getSmooth()](#getSmooth--) | 表示曲线平滑。 |
| [getSplitType()](#getSplitType--) | 返回或设置一个值，用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。 |
| [getSplitValue()](#getSplitValue--) | 返回或设置一个值，该值用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。 |
| [getTrendLines()](#getTrendLines--) | 返回此系列的所有趋势线。 |
| [getType()](#getType--) | 获取数据系列的类型。 |
| [getUpBars()](#getUpBars--) | 返回一个 DropBars 对象，表示折线图上的上升条。 |
| [getValues()](#getValues--) | 表示此图表系列的 Y 值。 |
| [getValuesFormatCode()](#getValuesFormatCode--) | 表示 Values NumberList 的格式代码。 |
| [getXErrorBar()](#getXErrorBar--) | 表示系列的 X 方向误差线。 |
| [getXValues()](#getXValues--) | 表示此图表系列的 X 值。 |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | 表示 X Values 的 NumberList 的格式代码。 |
| [getYErrorBar()](#getYErrorBar--) | 表示系列的 Y 方向误差线。 |
| [hasDropLines()](#hasDropLines--) | 如果图表有下拉线，则为 True。 |
| [hasHiLoLines()](#hasHiLoLines--) | 如果折线图具有高低线，则为 True。 |
| [hasLeaderLines()](#hasLeaderLines--) | 如果系列具有引线，则为 True。 |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | 如果雷达图具有类别轴标签，则为 True。 |
| [hasSeriesLines()](#hasSeriesLines--) | 如果堆积柱形图或条形图具有系列线，或如果饼形图的饼图或条形图的饼图在两个部分之间有连接线，则为 True。 |
| [hasUpDownBars()](#hasUpDownBars--) | 如果折线图具有上下条，则为 True。 |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | 指示阈值是否为自动。 |
| [isColorVaried()](#isColorVaried--) | 表示点的颜色是否多样化。 |
| [isFiltered()](#isFiltered--) | 指示系列是否已选择或已过滤。 |
| [isVerticalValues()](#isVerticalValues--) | 指示数据源是否为垂直方向。 |
| [move(int count)](#move-int-) | 将系列向上或向下移动。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | 设置与 3-D 条形图或柱形图一起使用的 3D 形状类型。 |
| [setBubbleScale(int value)](#setBubbleScale-int-) | 设置指定图表组中气泡的比例因子。 |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | 获取气泡图中气泡大小所表示的含义。 |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | 设置图表系列的气泡大小值。 |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | 表示点的颜色是否多样化。 |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | 返回或设置环形图组中孔的大小。 |
| [setExplosion(int value)](#setExplosion-int-) | 打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。 |
| [setFiltered(boolean value)](#setFiltered-boolean-) | 指示系列是否已选择或已过滤。 |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | 设置第一个饼图或环形图切片的角度，单位为度（顺时针从垂直方向起）。 |
| [setGapWidth(short value)](#setGapWidth-short-) | 返回或设置条形或柱形簇之间的间距，作为条形或柱形宽度的百分比。 |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | 如果系列具有三维外观，则为 True。 |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | 如果图表有下拉线，则为 True。 |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | 如果折线图具有高低线，则为 True。 |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | 如果系列具有引线，则为 True。 |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | 如果雷达图具有类别轴标签，则为 True。 |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | 如果堆积柱形图或条形图具有系列线，或如果饼形图的饼图或条形图的饼图在两个部分之间有连接线，则为 True。 |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | 如果折线图具有上下条，则为 True。 |
| [setName(String value)](#setName-java.lang.String-) | 设置数据系列的名称。 |
| [setOverlap(short value)](#setOverlap-short-) | 指定条形和柱形的定位方式。 |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | 指示此系列是否绘制在第二值轴上。 |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | 返回或设置饼图中的饼图或条形饼图的次要部分的大小，作为主饼图大小的百分比。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 如果系列具有阴影，则为 True。 |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | 如果为图表组显示负气泡，则为 True。 |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | 设置气泡图中气泡大小所表示的含义。 |
| [setSmooth(boolean value)](#setSmooth-boolean-) | 表示曲线平滑。 |
| [setSplitType(int value)](#setSplitType-int-) | 返回或设置一个值，用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。 |
| [setSplitValue(double value)](#setSplitValue-double-) | 返回或设置一个值，该值用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。 |
| [setType(int value)](#setType-int-) | 设置数据系列的类型。 |
| [setValues(String value)](#setValues-java.lang.String-) | 表示此图表系列的 Y 值。 |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | 表示 Values NumberList 的格式代码。 |
| [setXValues(String value)](#setXValues-java.lang.String-) | 表示此图表系列的 X 值。 |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | 表示 X Values 的 NumberList 的格式代码。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArea() {#getArea--}
```
public Area getArea()
```


表示 Series 对象的背景区域。

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


获取在 3-D 条形图或柱形图中使用的 3D 形状类型。

参见 [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype)。

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


表示 Series 对象的边框。

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


获取指定图表组中气泡的比例因子。它可以是 0（零）到 300 的整数值，对应默认大小的百分比。仅适用于气泡图。

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


获取气泡图中气泡大小所表示的含义。

参见 [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents)。

**Remarks**

注意：此成员现已过时。请改用 Aspose.Cells.Charts.Series.SizeRepresents 属性。该属性将在自 2012 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


获取图表系列的气泡大小值。

**Remarks**

仅适用于 [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) 或 [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D)。

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


获取系列的缓存类别值

**Remarks**

注意：此属性目前仅供内部使用。它将在下一个版本中被更改或移除。

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


获取系列的缓存值

**Remarks**

注意：此属性目前仅供内部使用。它将在下一个版本中被更改或移除。

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


获取用于在图表中绘制此系列每个点的实际类别值。

**Remarks**

此属性提供了一种便捷方式来获取由 [getXValues()](../../com.aspose.cells/series\#getXValues--) 定义的数据的实际值，尤其是当指定的数据源是外部链接、公式等时。

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


获取数据值的数量。

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


表示指定 ASeries 的 DataLabels 对象。

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


获取在图表中显示的系列名称。

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


返回或设置环形图组中孔的大小。孔的大小以图表大小的百分比表示，范围在 10% 到 90% 之间。

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


返回一个表示折线图中下垂条的 [DropBars](../../com.aspose.cells/dropbars) 对象。仅适用于折线图。

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


返回一个表示折线图或面积图中系列下垂线的 [Line](../../com.aspose.cells/line) 对象。仅适用于折线图或面积图。

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


获取第一个饼图或环形图切片的角度，单位为度（从垂直方向顺时针）。仅适用于饼图、3-D 饼图和环形图，取值范围为 0 到 360。

**Returns:**
短
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


返回或设置条形或柱形簇之间的间距，以条形或柱形宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Returns:**
短
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


如果系列具有三维外观，则为 True。

**Remarks**

仅适用于 [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) 或 [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) 图表。

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


返回一个 HiLoLines 对象，表示折线图中系列的高低线。仅适用于折线图。

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


表示布局的属性。

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


表示图表上的引导线。引导线将数据标签连接到数据点。此对象不是集合；没有表示单个引导线的对象。

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


获取对应此系列的图例项。

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


获取 [getMarker()](../../com.aspose.cells/series\#getMarker--)。

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


获取数据系列的名称。

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


指定条形和柱形的定位方式。取值范围为 -100 到 100。仅适用于二维条形图和二维柱形图。

**Returns:**
短
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


指示此系列是否绘制在第二值轴上。

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


获取用于在图表中绘制此系列每个点的实际值。

**Remarks**

此属性提供了一种便捷方式来获取由 [getValues()](../../com.aspose.cells/series\#getValues--) 定义的数据对应的实际值，尤其是当指定的数据源为外部链接、公式等时。

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


获取图表中系列的点集合。

**Remarks**

当图表为饼中饼或条形饼图时，最后一个点是第一个饼图中的其他点。

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


返回或设置饼中饼图或条形饼图的次要部分的大小，作为主饼图大小的百分比。取值范围为 5 到 200。

**Returns:**
短
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


返回一个 SeriesLines 对象，表示堆叠条形图或堆叠柱形图的系列线。仅适用于堆叠条形图和堆叠柱形图。

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


如果系列具有阴影，则为 True。

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


获取 [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) 对象，该对象保存系列的可视形状属性。

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


如果为图表组显示负气泡则为 true。仅对气泡图有效。

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


获取气泡图中气泡大小所表示的含义。

参见 [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents)。

**Remarks**

BubbleSizeRepresents.SizeIsArea 表示值 [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) 是气泡的面积。BubbleSizeRepresents.SizeIsWidth 表示值 [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) 是气泡的宽度。

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


表示曲线平滑。若对折线图或散点图启用了曲线平滑，则为 true。仅适用于折线图和带线的散点图。

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


返回或设置一个值，用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。

参见 [ChartSplitType](../../com.aspose.cells/chartsplittype)。

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


返回或设置一个值，该值用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


返回此系列的所有趋势线。

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


获取数据系列的类型。

参见 [ChartType](../../com.aspose.cells/charttype)。

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


返回一个 DropBars 对象，表示折线图上的上升柱。仅适用于折线图。

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


表示此图表系列的 Y 值。

**Remarks**

要获取此属性定义的实际值（对应此系列的每个点），请使用 [getPointValues()](../../com.aspose.cells/series\#getPointValues--)。

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


表示 Values NumberList 的格式代码。

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


表示系列的 X 方向误差线。

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


表示此图表系列的 X 值。

**Remarks**

仅适用于散点图和气泡图。对于其他类型的图表，请使用 [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--)；[getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) 用于获取此系列的实际类别值。

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


表示 X Values 的 NumberList 的格式代码。

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


表示系列的 Y 方向误差线。

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


如果图表具有下垂线则为 true。仅适用于折线图或面积图。

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


如果折线图具有高低线则为 true。仅适用于折线图。

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


如果系列具有引线，则为 True。

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


如果雷达图具有类目轴标签则为 true。仅适用于雷达图。

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


如果堆叠柱形图或条形图具有系列线，或饼中饼图或条形饼图在两个部分之间有连接线，则为 true。仅适用于堆叠柱形图、条形图、饼中饼图或条形饼图。

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


如果折线图具有上下柱则为 true。仅适用于折线图。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


指示阈值是否为自动。

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


表示点的颜色是否多变。图表必须仅包含一个系列或为饼图。

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


指示系列是否被选中或过滤。true 表示该系列已被过滤，且不会在图表中显示。

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


指示数据源是否为垂直方向。

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


将系列向上或向下移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 计数 | int | 移动的上下数量。如果小于零则将系列上移；如果大于零则将系列下移。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


设置与 3-D 条形图或柱形图一起使用的 3D 形状类型。

参见 [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


设置指定图表组中气泡的比例因子。它可以是 0（零）到 300 的整数值，对应默认大小的百分比。仅适用于气泡图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


获取气泡图中气泡大小所表示的含义。

参见 [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents)。

**Remarks**

注意：此成员现已过时。请改用 Aspose.Cells.Charts.Series.SizeRepresents 属性。该属性将在自 2012 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


设置图表系列的气泡大小值。

**Remarks**

仅适用于 [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) 或 [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


表示点的颜色是否多变。图表必须仅包含一个系列或为饼图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


返回或设置环形图组中孔的大小。孔的大小以图表大小的百分比表示，范围在 10% 到 90% 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


打开的饼图切片距离饼图中心的距离以饼图直径的百分比表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


指示系列是否被选中或过滤。true 表示该系列已被过滤，且不会在图表中显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


设置第一块饼图或环形图切片的角度，单位为度（顺时针从垂直方向）。仅适用于饼图、3D 饼图和环形图，取值范围为 0 到 360。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


返回或设置条形或柱形簇之间的间距，以条形或柱形宽度的百分比表示。此属性的值必须在 0 到 500 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


如果系列具有三维外观，则为 True。

**Remarks**

仅适用于 [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) 或 [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) 图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


如果图表具有下垂线则为 true。仅适用于折线图或面积图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


如果折线图具有高低线则为 true。仅适用于折线图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


如果系列具有引线，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


如果雷达图具有类目轴标签则为 true。仅适用于雷达图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


如果堆叠柱形图或条形图具有系列线，或饼中饼图或条形饼图在两个部分之间有连接线，则为 true。仅适用于堆叠柱形图、条形图、饼中饼图或条形饼图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


如果折线图具有上下柱则为 true。仅适用于折线图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置数据系列的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


指定条形和柱形的定位方式。取值范围为 -100 到 100。仅适用于二维条形图和二维柱形图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


指示此系列是否绘制在第二值轴上。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


返回或设置饼中饼图或条形饼图的次要部分的大小，作为主饼图大小的百分比。取值范围为 5 到 200。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


如果系列具有阴影，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


如果为图表组显示负气泡则为 true。仅对气泡图有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


设置气泡图中气泡大小所表示的含义。

参见 [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents)。

**Remarks**

BubbleSizeRepresents.SizeIsArea 表示值 [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) 是气泡的面积。BubbleSizeRepresents.SizeIsWidth 表示值 [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) 是气泡的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


表示曲线平滑。若对折线图或散点图启用了曲线平滑，则为 true。仅适用于折线图和带线的散点图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


返回或设置一个值，用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。

参见 [ChartSplitType](../../com.aspose.cells/chartsplittype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


返回或设置一个值，该值用于确定在饼图中的饼图或条形饼图中哪些数据点位于第二个饼或条。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置数据系列的类型。

参见 [ChartType](../../com.aspose.cells/charttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


表示此图表系列的 Y 值。

**Remarks**

要获取此属性定义的实际值（对应此系列的每个点），请使用 [getPointValues()](../../com.aspose.cells/series\#getPointValues--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


表示 Values NumberList 的格式代码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


表示此图表系列的 X 值。

**Remarks**

仅适用于散点图和气泡图。对于其他类型的图表，请使用 [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--)；[getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) 用于获取此系列的实际类别值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


表示 X Values 的 NumberList 的格式代码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

