---
title: Series
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single data series in a chart.
type: docs
url: /java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Encapsulates the object that represents a single data series in a chart.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Represents the background area of Series object. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Gets the 3D shape type used with the 3-D bar or column chart. |
| [getBorder()](#getBorder--) | Represents border of Series object. |
| [getBubbleScale()](#getBubbleScale--) | Gets the scale factor for bubbles in the specified chart group. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Gets what the bubble size represents on a bubble chart. |
| [getBubbleSizes()](#getBubbleSizes--) | Gets the bubble sizes values of the chart series. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Gets the cached category values for the series |
| [getCachedValues()](#getCachedValues--) | Gets the cached values for the series |
| [getCategoryValues()](#getCategoryValues--) | Gets the actual category values that are used to plot every point of this series in the chart. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Gets the number of the data values. |
| [getDataLabels()](#getDataLabels--) | Represents the DataLabels object for the specified ASeries. |
| [getDisplayName()](#getDisplayName--) | Gets the series's name that displays on the chart graph. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Returns or sets the size of the hole in a doughnut chart group. |
| [getDownBars()](#getDownBars--) | Returns a [DropBars](../../com.aspose.cells/dropbars) object that represents the down bars on a line chart. |
| [getDropLines()](#getDropLines--) | Returns a [Line](../../com.aspose.cells/line) object that represents the drop lines for a series on the line chart or area chart. |
| [getExplosion()](#getExplosion--) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Gets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). |
| [getGapWidth()](#getGapWidth--) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. |
| [getHas3DEffect()](#getHas3DEffect--) | True if the series has a three-dimensional appearance. |
| [getHiLoLines()](#getHiLoLines--) | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. |
| [getLayoutProperties()](#getLayoutProperties--) | Represents the properties of layout. |
| [getLeaderLines()](#getLeaderLines--) | Represents leader lines on a chart. |
| [getLegendEntry()](#getLegendEntry--) | Gets the legend entry according to this series. |
| [getMarker()](#getMarker--) | Gets the [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Gets the name of the data series. |
| [getOverlap()](#getOverlap--) | Specifies how bars and columns are positioned. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indicates if this series is plotted on second value axis. |
| [getPointValues()](#getPointValues--) | Gets the actual values that are used to plot every point of this series in the chart. |
| [getPoints()](#getPoints--) | Gets the collection of points in a series in a chart. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. |
| [getSeriesLines()](#getSeriesLines--) | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. |
| [getShadow()](#getShadow--) | True if the series has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) object that holds the visual shape properties of the Series. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | True if negative bubbles are shown for the chart group. |
| [getSizeRepresents()](#getSizeRepresents--) | Gets what the bubble size represents on a bubble chart. |
| [getSmooth()](#getSmooth--) | Represents curve smoothing. |
| [getSplitType()](#getSplitType--) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getSplitValue()](#getSplitValue--) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getTrendLines()](#getTrendLines--) | Returns all the trendlines of this series. |
| [getType()](#getType--) | Gets a data series' type. |
| [getUpBars()](#getUpBars--) | Returns an DropBars object that represents the up bars on a line chart. |
| [getValues()](#getValues--) | Represents the Y values of this chart series. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Represents format code of Values's NumberList. |
| [getXErrorBar()](#getXErrorBar--) | Represents X direction error bar of the series. |
| [getXValues()](#getXValues--) | Represents the X values of this chart series. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Represents format code of X Values's NumberList. |
| [getYErrorBar()](#getYErrorBar--) | Represents Y direction error bar of the series. |
| [hasDropLines()](#hasDropLines--) | True if the chart has drop lines. |
| [hasHiLoLines()](#hasHiLoLines--) | True if the line chart has high-low lines. |
| [hasLeaderLines()](#hasLeaderLines--) | True if the series has leader lines. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | True if a radar chart has category axis labels. |
| [hasSeriesLines()](#hasSeriesLines--) | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. |
| [hasUpDownBars()](#hasUpDownBars--) | True if a line chart has up and down bars. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Indicates whether the threshold value is automatic. |
| [isColorVaried()](#isColorVaried--) | Represents if the color of points is varied. |
| [isFiltered()](#isFiltered--) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [isVerticalValues()](#isVerticalValues--) | Indicates whether the data source is vertical. |
| [move(int count)](#move-int-) | Moves the series up or down. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Sets the 3D shape type used with the 3-D bar or column chart. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Sets the scale factor for bubbles in the specified chart group. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Gets what the bubble size represents on a bubble chart. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Sets the bubble sizes values of the chart series. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Represents if the color of points is varied. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Returns or sets the size of the hole in a doughnut chart group. |
| [setExplosion(int value)](#setExplosion-int-) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). |
| [setGapWidth(short value)](#setGapWidth-short-) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | True if the series has a three-dimensional appearance. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | True if the chart has drop lines. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | True if the line chart has high-low lines. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | True if the series has leader lines. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | True if a radar chart has category axis labels. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | True if a line chart has up and down bars. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the data series. |
| [setOverlap(short value)](#setOverlap-short-) | Specifies how bars and columns are positioned. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Indicates if this series is plotted on second value axis. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the series has a shadow. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | True if negative bubbles are shown for the chart group. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Sets what the bubble size represents on a bubble chart. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Represents curve smoothing. |
| [setSplitType(int value)](#setSplitType-int-) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setSplitValue(double value)](#setSplitValue-double-) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setType(int value)](#setType-int-) | Sets a data series' type. |
| [setValues(String value)](#setValues-java.lang.String-) | Represents the Y values of this chart series. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Represents format code of Values's NumberList. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Represents the X values of this chart series. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Represents format code of X Values's NumberList. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Represents the background area of Series object.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Gets the 3D shape type used with the 3-D bar or column chart.

See [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Represents border of Series object.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Gets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Gets what the bubble size represents on a bubble chart.

See [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Gets the bubble sizes values of the chart series.

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Gets the cached category values for the series

**Remarks**

NOTE: This property is currently for internal use only. It will be changed or removed in next version.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Gets the cached values for the series

**Remarks**

NOTE: This property is currently for internal use only. It will be changed or removed in next version.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Gets the actual category values that are used to plot every point of this series in the chart.

**Remarks**

This property provides one convenient way to get the actual values corresponding to the data defined by [getXValues()](../../com.aspose.cells/series\#getXValues--), especially when the specified data source is external link, formula, ...etc.

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


Gets the number of the data values.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Represents the DataLabels object for the specified ASeries.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Gets the series's name that displays on the chart graph.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Returns a [DropBars](../../com.aspose.cells/dropbars) object that represents the down bars on a line chart. Applies only to line charts.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Returns a [Line](../../com.aspose.cells/line) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Gets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


True if the series has a three-dimensional appearance. Applies only to bubble charts.

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Represents the properties of layout.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn\\u9225\\u6a9b a collection; there\\u9225\\u6a9a no object that represents a single leader line.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Gets the legend entry according to this series.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Gets the [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Gets the name of the data series.

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


Specifies how bars and columns are positioned. Can be a value between \\u9225?100 and 100. Applies only to 2-D bar and 2-D column charts.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Indicates if this series is plotted on second value axis.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Gets the actual values that are used to plot every point of this series in the chart.

**Remarks**

This property provides one convenient way to get the actual values corresponding to the data defined by [getValues()](../../com.aspose.cells/series\#getValues--), especially when the specified data source is external link, formula, ...etc.

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


Gets the collection of points in a series in a chart.

**Remarks**

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True if the series has a shadow.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Gets the [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) object that holds the visual shape properties of the Series.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


True if negative bubbles are shown for the chart group. Valid only for bubble charts.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Gets what the bubble size represents on a bubble chart.

See [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the width of the bubble.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

See [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Returns all the trendlines of this series.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Gets a data series' type.

See [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Represents the Y values of this chart series.

**Remarks**

To get the actual values(corresponding to every point of this series) defined by this property, please use [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Represents format code of Values's NumberList.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Represents X direction error bar of the series.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Represents the X values of this chart series.

**Remarks**

To get the actual values(corresponding to every point of this series) defined by this property, please use [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--).

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Represents format code of X Values's NumberList.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Represents Y direction error bar of the series.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


True if the chart has drop lines. Applies only to line chart or area charts.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


True if the line chart has high-low lines. Applies only to line charts.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


True if the series has leader lines.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


True if a radar chart has category axis labels. Applies only to radar charts.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


True if a line chart has up and down bars. Applies only to line charts.

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


Indicates whether the threshold value is automatic.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Represents if the color of points is varied. The chart must contain only one series.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Indicates whether the data source is vertical.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Moves the series up or down.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | int | The number of moving up or down. Move the series up if this is less than zero; Move the series down if this is greater than zero. |

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


Sets the 3D shape type used with the 3-D bar or column chart.

See [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Gets what the bubble size represents on a bubble chart.

See [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Sets the bubble sizes values of the chart series.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Represents if the color of points is varied. The chart must contain only one series.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


True if the series has a three-dimensional appearance. Applies only to bubble charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


True if the chart has drop lines. Applies only to line chart or area charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


True if the line chart has high-low lines. Applies only to line charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


True if the series has leader lines.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


True if a radar chart has category axis labels. Applies only to radar charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


True if a line chart has up and down bars. Applies only to line charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sets the name of the data series.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Specifies how bars and columns are positioned. Can be a value between \\u9225?100 and 100. Applies only to 2-D bar and 2-D column charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Indicates if this series is plotted on second value axis.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True if the series has a shadow.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


True if negative bubbles are shown for the chart group. Valid only for bubble charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Sets what the bubble size represents on a bubble chart.

See [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the width of the bubble.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

See [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Sets a data series' type.

See [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Represents the Y values of this chart series.

**Remarks**

To get the actual values(corresponding to every point of this series) defined by this property, please use [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Represents format code of Values's NumberList.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Represents the X values of this chart series.

**Remarks**

To get the actual values(corresponding to every point of this series) defined by this property, please use [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Represents format code of X Values's NumberList.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

