---
title: "Series"
linktitle: "Series"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a single data series in a chart."
type: docs
weight: 3480
url: /nodejs/aspose.cells/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

## Methods

| Name | Description |
| --- | --- |
| [getArea()](#getarea) | Represents the background area of Series object. |
| [getBar3DShapeType()](#getbar3dshapetype) | Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType intege |
| [getBorder()](#getborder) | Represents border of Series object. |
| [getBubbleScale()](#getbubblescale) | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, |
| [getBubbleSizeRepresents()](#getbubblesizerepresents) | Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer consta |
| [getBubbleSizes()](#getbubblesizes) | Gets or sets the bubble sizes values of the chart series. |
| [getCachedCategoryValues()](#getcachedcategoryvalues) |  |
| [getCachedValues()](#getcachedvalues) |  |
| [getCategoryValues()](#getcategoryvalues) |  |
| [getCountOfDataValues()](#getcountofdatavalues) | Gets the number of the data values. |
| [getDataLabels()](#getdatalabels) | Represents the DataLabels object for the specified ASeries. |
| [getDisplayName()](#getdisplayname) | Gets the series's name that displays on the chart graph. |
| [getDoughnutHoleSize()](#getdoughnutholesize) | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart  |
| [getDownBars()](#getdownbars) | Returns a DropBars object that represents the down bars on a line chart. Applies only to line charts. |
| [getDropLines()](#getdroplines) | Returns a Line object that represents the drop lines for a series on the line chart or area chart. Applies only to line  |
| [getExplosion()](#getexplosion) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getFirstSliceAngle()](#getfirstsliceangle) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [getGapWidth()](#getgapwidth) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [getHas3DEffect()](#gethas3deffect) | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [getHiLoLines()](#gethilolines) | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [getLayoutProperties()](#getlayoutproperties) | Represents the properties of layout. |
| [getLeaderLines()](#getleaderlines) | Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; the |
| [getLegendEntry()](#getlegendentry) | Gets the legend entry according to this series. |
| [getMarker()](#getmarker) | Gets the Marker. |
| [getName()](#getname) | Gets or sets the name of the data series. |
| [getOverlap()](#getoverlap) | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D col |
| [getPlotOnSecondAxis()](#getplotonsecondaxis) | Indicates if this series is plotted on second value axis. |
| [getPointValues()](#getpointvalues) |  |
| [getPoints()](#getpoints) | Gets the collection of points in a series in a chart. When the chart is Pie of Pie or Bar of Pie, the last point is othe |
| [getSecondPlotSize()](#getsecondplotsize) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of |
| [getSeriesLines()](#getserieslines) | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies |
| [getShadow()](#getshadow) | True if the series has a shadow. |
| [getShapeProperties()](#getshapeproperties) | Gets the ShapePropertyCollection object that holds the visual shape properties of the Series. |
| [getShowNegativeBubbles()](#getshownegativebubbles) | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [getSizeRepresents()](#getsizerepresents) | Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents intege |
| [getSmooth()](#getsmooth) | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to li |
| [getSplitType()](#getsplittype) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of p |
| [getSplitValue()](#getsplitvalue) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie o |
| [getTrendLines()](#gettrendlines) | Returns all the trendlines of this series. |
| [getType()](#gettype) | Gets or sets a data series' type. The value of the property is ChartType integer constant. |
| [getUpBars()](#getupbars) | Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [getValues()](#getvalues) | Represents the Y values of this chart series. |
| [getValuesFormatCode()](#getvaluesformatcode) | Represents format code of Values's NumberList. |
| [getXErrorBar()](#getxerrorbar) | Represents X direction error bar of the series. |
| [getXValues()](#getxvalues) | Represents the x values of the chart series. |
| [getXValuesFormatCode()](#getxvaluesformatcode) |  |
| [getYErrorBar()](#getyerrorbar) | Represents Y direction error bar of the series. |
| [hasDropLines()](#hasdroplines) | True if the chart has drop lines. Applies only to line chart or area charts. |
| [hasHiLoLines()](#hashilolines) | True if the line chart has high-low lines. Applies only to line charts. |
| [hasLeaderLines()](#hasleaderlines) | True if the series has leader lines. |
| [hasRadarAxisLabels()](#hasradaraxislabels) | True if a radar chart has category axis labels. Applies only to radar charts. |
| [hasSeriesLines()](#hasserieslines) | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector  |
| [hasUpDownBars()](#hasupdownbars) | True if a line chart has up and down bars. Applies only to line charts. |
| [isAutoSplit()](#isautosplit) | Indicates whether the threshold value is automatic. |
| [isColorVaried()](#iscolorvaried) | Represents if the color of points is varied. The chart must contain only one series. |
| [isFiltered()](#isfiltered) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be display |
| [isVerticalValues()](#isverticalvalues) | Indicates whether the data source is vertical. |
| [move(count)](#move) | Moves the series up or down. |
| [setBar3DShapeType()](#setbar3dshapetype) | Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType intege |
| [setBubbleScale()](#setbubblescale) | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, |
| [setBubbleSizeRepresents()](#setbubblesizerepresents) | Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer consta |
| [setBubbleSizes()](#setbubblesizes) | Gets or sets the bubble sizes values of the chart series. |
| [setColorVaried()](#setcolorvaried) | Represents if the color of points is varied. The chart must contain only one series. |
| [setDoughnutHoleSize()](#setdoughnutholesize) | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart  |
| [setExplosion()](#setexplosion) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setFiltered()](#setfiltered) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be display |
| [setFirstSliceAngle()](#setfirstsliceangle) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [setGapWidth()](#setgapwidth) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [setHas3DEffect()](#sethas3deffect) | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [setHasDropLines()](#sethasdroplines) | True if the chart has drop lines. Applies only to line chart or area charts. |
| [setHasHiLoLines()](#sethashilolines) | True if the line chart has high-low lines. Applies only to line charts. |
| [setHasLeaderLines()](#sethasleaderlines) | True if the series has leader lines. |
| [setHasRadarAxisLabels()](#sethasradaraxislabels) | True if a radar chart has category axis labels. Applies only to radar charts. |
| [setHasSeriesLines()](#sethasserieslines) | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector  |
| [setHasUpDownBars()](#sethasupdownbars) | True if a line chart has up and down bars. Applies only to line charts. |
| [setName()](#setname) | Gets or sets the name of the data series. |
| [setOverlap()](#setoverlap) | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D col |
| [setPlotOnSecondAxis()](#setplotonsecondaxis) | Indicates if this series is plotted on second value axis. |
| [setSecondPlotSize()](#setsecondplotsize) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of |
| [setShadow()](#setshadow) | True if the series has a shadow. |
| [setShowNegativeBubbles()](#setshownegativebubbles) | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [setSizeRepresents()](#setsizerepresents) | Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents intege |
| [setSmooth()](#setsmooth) | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to li |
| [setSplitType()](#setsplittype) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of p |
| [setSplitValue()](#setsplitvalue) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie o |
| [setType()](#settype) | Gets or sets a data series' type. The value of the property is ChartType integer constant. |
| [setValues()](#setvalues) | Represents the Y values of this chart series. |
| [setValuesFormatCode()](#setvaluesformatcode) | Represents format code of Values's NumberList. |
| [setXValues()](#setxvalues) | Represents the x values of the chart series. |
| [setXValuesFormatCode()](#setxvaluesformatcode) |  |

### getArea() {#getarea}

Represents the background area of Series object.

### getBar3DShapeType() {#getbar3dshapetype}

Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType integer constant.

### getBorder() {#getborder}

Represents border of Series object.

### getBubbleScale() {#getbubblescale}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

### getBubbleSizeRepresents() {#getbubblesizerepresents}

Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. the bubble size represents on a bubble chart. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getBubbleSizes() {#getbubblesizes}

Gets or sets the bubble sizes values of the chart series.

### getCachedCategoryValues() {#getcachedcategoryvalues}

### getCachedValues() {#getcachedvalues}

### getCategoryValues() {#getcategoryvalues}

### getCountOfDataValues() {#getcountofdatavalues}

Gets the number of the data values.

### getDataLabels() {#getdatalabels}

Represents the DataLabels object for the specified ASeries.

### getDisplayName() {#getdisplayname}

Gets the series's name that displays on the chart graph.

### getDoughnutHoleSize() {#getdoughnutholesize}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

### getDownBars() {#getdownbars}

Returns a DropBars object that represents the down bars on a line chart. Applies only to line charts.

### getDropLines() {#getdroplines}

Returns a Line object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

### getExplosion() {#getexplosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

### getFirstSliceAngle() {#getfirstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

### getGapWidth() {#getgapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

### getHas3DEffect() {#gethas3deffect}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

### getHiLoLines() {#gethilolines}

Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

### getLayoutProperties() {#getlayoutproperties}

Represents the properties of layout.

### getLeaderLines() {#getleaderlines}

Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

### getLegendEntry() {#getlegendentry}

Gets the legend entry according to this series.

### getMarker() {#getmarker}

Gets the Marker.

### getName() {#getname}

Gets or sets the name of the data series.

**Example:**

```js
//Reference name to a cell
chart.getNSeries().get(0).setName("=A1");
//Set a string to name
chart.getNSeries().get(0).setName("First Series");
```

### getOverlap() {#getoverlap}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

### getPlotOnSecondAxis() {#getplotonsecondaxis}

Indicates if this series is plotted on second value axis.

### getPointValues() {#getpointvalues}

### getPoints() {#getpoints}

Gets the collection of points in a series in a chart. When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### getSecondPlotSize() {#getsecondplotsize}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

### getSeriesLines() {#getserieslines}

Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

### getShadow() {#getshadow}

True if the series has a shadow.

### getShapeProperties() {#getshapeproperties}

Gets the ShapePropertyCollection object that holds the visual shape properties of the Series.

### getShowNegativeBubbles() {#getshownegativebubbles}

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

### getSizeRepresents() {#getsizerepresents}

Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. BubbleSizeRepresents.SizeIsArea means the value BubbleSizes is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value BubbleSizes is the width of the bubble.

### getSmooth() {#getsmooth}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

### getSplitType() {#getsplittype}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. The value of the property is ChartSplitType integer constant.

### getSplitValue() {#getsplitvalue}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

### getTrendLines() {#gettrendlines}

Returns all the trendlines of this series.

### getType() {#gettype}

Gets or sets a data series' type. The value of the property is ChartType integer constant.

### getUpBars() {#getupbars}

Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

### getValues() {#getvalues}

Represents the Y values of this chart series.

### getValuesFormatCode() {#getvaluesformatcode}

Represents format code of Values's NumberList.

### getXErrorBar() {#getxerrorbar}

Represents X direction error bar of the series.

### getXValues() {#getxvalues}

Represents the x values of the chart series.

### getXValuesFormatCode() {#getxvaluesformatcode}

### getYErrorBar() {#getyerrorbar}

Represents Y direction error bar of the series.

### hasDropLines() {#hasdroplines}

True if the chart has drop lines. Applies only to line chart or area charts.

### hasHiLoLines() {#hashilolines}

True if the line chart has high-low lines. Applies only to line charts.

### hasLeaderLines() {#hasleaderlines}

True if the series has leader lines.

### hasRadarAxisLabels() {#hasradaraxislabels}

True if a radar chart has category axis labels. Applies only to radar charts.

### hasSeriesLines() {#hasserieslines}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

### hasUpDownBars() {#hasupdownbars}

True if a line chart has up and down bars. Applies only to line charts.

### isAutoSplit() {#isautosplit}

Indicates whether the threshold value is automatic.

### isColorVaried() {#iscolorvaried}

Represents if the color of points is varied. The chart must contain only one series.

### isFiltered() {#isfiltered}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

### isVerticalValues() {#isverticalvalues}

Indicates whether the data source is vertical.

### move(count) {#move}

Moves the series up or down.

| Parameter | Type | Description |
| --- | --- | --- |
| count | Number | The number of moving up or down. Move the series up if this is less than zero; Move the series down if this is greater than zero. |

### setBar3DShapeType() {#setbar3dshapetype}

Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType integer constant.

### setBubbleScale() {#setbubblescale}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

### setBubbleSizeRepresents() {#setbubblesizerepresents}

Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. the bubble size represents on a bubble chart. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### setBubbleSizes() {#setbubblesizes}

Gets or sets the bubble sizes values of the chart series.

### setColorVaried() {#setcolorvaried}

Represents if the color of points is varied. The chart must contain only one series.

### setDoughnutHoleSize() {#setdoughnutholesize}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

### setExplosion() {#setexplosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

### setFiltered() {#setfiltered}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

### setFirstSliceAngle() {#setfirstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

### setGapWidth() {#setgapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

### setHas3DEffect() {#sethas3deffect}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

### setHasDropLines() {#sethasdroplines}

True if the chart has drop lines. Applies only to line chart or area charts.

### setHasHiLoLines() {#sethashilolines}

True if the line chart has high-low lines. Applies only to line charts.

### setHasLeaderLines() {#sethasleaderlines}

True if the series has leader lines.

### setHasRadarAxisLabels() {#sethasradaraxislabels}

True if a radar chart has category axis labels. Applies only to radar charts.

### setHasSeriesLines() {#sethasserieslines}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

### setHasUpDownBars() {#sethasupdownbars}

True if a line chart has up and down bars. Applies only to line charts.

### setName() {#setname}

Gets or sets the name of the data series.

**Example:**

```js
//Reference name to a cell
chart.getNSeries().get(0).setName("=A1");
//Set a string to name
chart.getNSeries().get(0).setName("First Series");
```

### setOverlap() {#setoverlap}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

### setPlotOnSecondAxis() {#setplotonsecondaxis}

Indicates if this series is plotted on second value axis.

### setSecondPlotSize() {#setsecondplotsize}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

### setShadow() {#setshadow}

True if the series has a shadow.

### setShowNegativeBubbles() {#setshownegativebubbles}

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

### setSizeRepresents() {#setsizerepresents}

Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. BubbleSizeRepresents.SizeIsArea means the value BubbleSizes is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value BubbleSizes is the width of the bubble.

### setSmooth() {#setsmooth}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

### setSplitType() {#setsplittype}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. The value of the property is ChartSplitType integer constant.

### setSplitValue() {#setsplitvalue}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

### setType() {#settype}

Gets or sets a data series' type. The value of the property is ChartType integer constant.

### setValues() {#setvalues}

Represents the Y values of this chart series.

### setValuesFormatCode() {#setvaluesformatcode}

Represents format code of Values's NumberList.

### setXValues() {#setxvalues}

Represents the x values of the chart series.

### setXValuesFormatCode() {#setxvaluesformatcode}
