---
title: Series
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single data series in a chart.
type: docs
weight: 490
url: /java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Encapsulates the object that represents a single data series in a chart.

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
| [getBar3DShapeType()](#getBar3DShapeType--) | the 3D shape type used with the 3-D bar or column chart. |
| [getBarShape()](#getBarShape--) | the 3D shape type used with the 3-D bar or column chart. |
| [getBorder()](#getBorder--) | Represents border of Series object. |
| [getBubbleScale()](#getBubbleScale--) | the scale factor for bubbles in the specified chart group. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Gets what the bubble size represents on a bubble chart. |
| [getBubbleSizes()](#getBubbleSizes--) | the bubble sizes values of the chart series. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Gets the number of the data values. |
| [getDataLabels()](#getDataLabels--) | Represents the DataLabels object for the specified ASeries. |
| [getDisplayName()](#getDisplayName--) | Gets the series's name that displays on the chart graph. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Returns or sets the size of the hole in a doughnut chart group. |
| [getDownBars()](#getDownBars--) | Returns a [DropBars](../../com.aspose.cells/dropbars) object that represents the down bars on a line chart. |
| [getDropLines()](#getDropLines--) | Returns a [Line](../../com.aspose.cells/line) object that represents the drop lines for a series on the line chart or area chart. |
| [getExplosion()](#getExplosion--) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). |
| [getGapWidth()](#getGapWidth--) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. |
| [getHas3DEffect()](#getHas3DEffect--) | True if the series has a three-dimensional appearance. |
| [getHiLoLines()](#getHiLoLines--) | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. |
| [getLayoutProperties()](#getLayoutProperties--) | Represents the properties of layout. |
| [getLeaderLines()](#getLeaderLines--) | Represents leader lines on a chart. |
| [getLegendEntry()](#getLegendEntry--) | Gets the legend entry according to this series. |
| [getMarker()](#getMarker--) | Gets the [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | the name of the data series. |
| [getOverlap()](#getOverlap--) | Specifies how bars and columns are positioned. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indicates if this series is plotted on second value axis. |
| [getPoints()](#getPoints--) | Gets the collection of points in a series in a chart. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. |
| [getSeriesLines()](#getSeriesLines--) | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. |
| [getShadow()](#getShadow--) | True if the series has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) object that holds the visual shape properties of the Series. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | True if negative bubbles are shown for the chart group. |
| [getSizeRepresents()](#getSizeRepresents--) | what the bubble size represents on a bubble chart. |
| [getSmooth()](#getSmooth--) | Represents curve smoothing. |
| [getSplitType()](#getSplitType--) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getSplitValue()](#getSplitValue--) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getTrendLines()](#getTrendLines--) | Returns an object that represents a collection of all the trendlines for the series. |
| [getType()](#getType--) | a data series' type. |
| [getUpBars()](#getUpBars--) | Returns an DropBars object that represents the up bars on a line chart. |
| [getValues()](#getValues--) | Represents the data of the chart series. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Represents format code of Values\\u9225\\u69ae NumberList. |
| [getXErrorBar()](#getXErrorBar--) | Represents X direction error bar of the series. |
| [getXValues()](#getXValues--) | Represents the x values of the chart series. |
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
| [isVerticalValues()](#isVerticalValues--) | Indicates whether the data source is vertical. |
| [move(int count)](#move-int-) | Moves the series up or down. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | For the description of this property, please see [getBar3DShapeType()](../../com.aspose.cells/series\#getBar3DShapeType--) |
| [setBarShape(int value)](#setBarShape-int-) | For the description of this property, please see [getBarShape()](../../com.aspose.cells/series\#getBarShape--) |
| [setBubbleScale(int value)](#setBubbleScale-int-) | For the description of this property, please see [getBubbleScale()](../../com.aspose.cells/series\#getBubbleScale--) |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | For the description of this property, please see [getBubbleSizeRepresents()](../../com.aspose.cells/series\#getBubbleSizeRepresents--) |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | For the description of this property, please see [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | For the description of this property, please see [isColorVaried()](../../com.aspose.cells/series\#isColorVaried--) |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | For the description of this property, please see [getDoughnutHoleSize()](../../com.aspose.cells/series\#getDoughnutHoleSize--) |
| [setExplosion(int value)](#setExplosion-int-) | For the description of this property, please see [getExplosion()](../../com.aspose.cells/series\#getExplosion--) |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | For the description of this property, please see [getFirstSliceAngle()](../../com.aspose.cells/series\#getFirstSliceAngle--) |
| [setGapWidth(short value)](#setGapWidth-short-) | For the description of this property, please see [getGapWidth()](../../com.aspose.cells/series\#getGapWidth--) |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | For the description of this property, please see [getHas3DEffect()](../../com.aspose.cells/series\#getHas3DEffect--) |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | For the description of this property, please see [hasDropLines()](../../com.aspose.cells/series\#hasDropLines--) |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | For the description of this property, please see [hasHiLoLines()](../../com.aspose.cells/series\#hasHiLoLines--) |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | For the description of this property, please see [hasLeaderLines()](../../com.aspose.cells/series\#hasLeaderLines--) |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | For the description of this property, please see [hasRadarAxisLabels()](../../com.aspose.cells/series\#hasRadarAxisLabels--) |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | For the description of this property, please see [hasSeriesLines()](../../com.aspose.cells/series\#hasSeriesLines--) |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | For the description of this property, please see [hasUpDownBars()](../../com.aspose.cells/series\#hasUpDownBars--) |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.cells/series\#getName--) |
| [setOverlap(short value)](#setOverlap-short-) | For the description of this property, please see [getOverlap()](../../com.aspose.cells/series\#getOverlap--) |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | For the description of this property, please see [getPlotOnSecondAxis()](../../com.aspose.cells/series\#getPlotOnSecondAxis--) |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | For the description of this property, please see [getSecondPlotSize()](../../com.aspose.cells/series\#getSecondPlotSize--) |
| [setShadow(boolean value)](#setShadow-boolean-) | For the description of this property, please see [getShadow()](../../com.aspose.cells/series\#getShadow--) |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | For the description of this property, please see [getShowNegativeBubbles()](../../com.aspose.cells/series\#getShowNegativeBubbles--) |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | For the description of this property, please see [getSizeRepresents()](../../com.aspose.cells/series\#getSizeRepresents--) |
| [setSmooth(boolean value)](#setSmooth-boolean-) | For the description of this property, please see [getSmooth()](../../com.aspose.cells/series\#getSmooth--) |
| [setSplitType(int value)](#setSplitType-int-) | For the description of this property, please see [getSplitType()](../../com.aspose.cells/series\#getSplitType--) |
| [setSplitValue(double value)](#setSplitValue-double-) | For the description of this property, please see [getSplitValue()](../../com.aspose.cells/series\#getSplitValue--) |
| [setType(int value)](#setType-int-) | For the description of this property, please see [getType()](../../com.aspose.cells/series\#getType--) |
| [setValues(String value)](#setValues-java.lang.String-) | For the description of this property, please see [getValues()](../../com.aspose.cells/series\#getValues--) |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | For the description of this property, please see [getValuesFormatCode()](../../com.aspose.cells/series\#getValuesFormatCode--) |
| [setXValues(String value)](#setXValues-java.lang.String-) | For the description of this property, please see [getXValues()](../../com.aspose.cells/series\#getXValues--) |
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


the 3D shape type used with the 3-D bar or column chart.

**Returns:**
int
### getBarShape() {#getBarShape--}
```
public int getBarShape()
```


the 3D shape type used with the 3-D bar or column chart. NOTE: This member is now obsolete. Instead, please use ASeries.Bar3DShapeType property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

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


the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Gets what the bubble size represents on a bubble chart. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


the bubble sizes values of the chart series.

**Returns:**
java.lang.String
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


the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

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


the name of the data series.

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
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Gets the collection of points in a series in a chart. When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

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


what the bubble size represents on a bubble chart. BubbleSizeRepresents.SizeIsArea means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) is the width of the bubble.

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


Returns an object that represents a collection of all the trendlines for the series.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


a data series' type.

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


Represents the data of the chart series.

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Represents format code of Values\\u9225\\u69ae NumberList.

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


Represents the x values of the chart series.

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


For the description of this property, please see [getBar3DShapeType()](../../com.aspose.cells/series\#getBar3DShapeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBarShape(int value) {#setBarShape-int-}
```
public void setBarShape(int value)
```


For the description of this property, please see [getBarShape()](../../com.aspose.cells/series\#getBarShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


For the description of this property, please see [getBubbleScale()](../../com.aspose.cells/series\#getBubbleScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


For the description of this property, please see [getBubbleSizeRepresents()](../../com.aspose.cells/series\#getBubbleSizeRepresents--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


For the description of this property, please see [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


For the description of this property, please see [isColorVaried()](../../com.aspose.cells/series\#isColorVaried--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


For the description of this property, please see [getDoughnutHoleSize()](../../com.aspose.cells/series\#getDoughnutHoleSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


For the description of this property, please see [getExplosion()](../../com.aspose.cells/series\#getExplosion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


For the description of this property, please see [getFirstSliceAngle()](../../com.aspose.cells/series\#getFirstSliceAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


For the description of this property, please see [getGapWidth()](../../com.aspose.cells/series\#getGapWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


For the description of this property, please see [getHas3DEffect()](../../com.aspose.cells/series\#getHas3DEffect--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


For the description of this property, please see [hasDropLines()](../../com.aspose.cells/series\#hasDropLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


For the description of this property, please see [hasHiLoLines()](../../com.aspose.cells/series\#hasHiLoLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


For the description of this property, please see [hasLeaderLines()](../../com.aspose.cells/series\#hasLeaderLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


For the description of this property, please see [hasRadarAxisLabels()](../../com.aspose.cells/series\#hasRadarAxisLabels--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


For the description of this property, please see [hasSeriesLines()](../../com.aspose.cells/series\#hasSeriesLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


For the description of this property, please see [hasUpDownBars()](../../com.aspose.cells/series\#hasUpDownBars--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.cells/series\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


For the description of this property, please see [getOverlap()](../../com.aspose.cells/series\#getOverlap--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


For the description of this property, please see [getPlotOnSecondAxis()](../../com.aspose.cells/series\#getPlotOnSecondAxis--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


For the description of this property, please see [getSecondPlotSize()](../../com.aspose.cells/series\#getSecondPlotSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


For the description of this property, please see [getShadow()](../../com.aspose.cells/series\#getShadow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


For the description of this property, please see [getShowNegativeBubbles()](../../com.aspose.cells/series\#getShowNegativeBubbles--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


For the description of this property, please see [getSizeRepresents()](../../com.aspose.cells/series\#getSizeRepresents--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


For the description of this property, please see [getSmooth()](../../com.aspose.cells/series\#getSmooth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


For the description of this property, please see [getSplitType()](../../com.aspose.cells/series\#getSplitType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


For the description of this property, please see [getSplitValue()](../../com.aspose.cells/series\#getSplitValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see [getType()](../../com.aspose.cells/series\#getType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


For the description of this property, please see [getValues()](../../com.aspose.cells/series\#getValues--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


For the description of this property, please see [getValuesFormatCode()](../../com.aspose.cells/series\#getValuesFormatCode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


For the description of this property, please see [getXValues()](../../com.aspose.cells/series\#getXValues--)

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

