---
title: "Chart Class"
linktitle: "Chart"
articleTitle: "Chart"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents a single Excel chart."
type: docs
weight: 710
url: /python-java/asposecells.api/chart/
---

## Chart class

Encapsulates the object that represents a single Excel chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Style](#style) | int | Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set. |
| [ChartObject](#chartobject) | ChartShape | Represents the chartShape; |
| [HidePivotFieldButtons](#hidepivotfieldbuttons) | boolean | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [PivotOptions](#pivotoptions) | PivotOptions | Specifies the pivot controls that appear on the chart |
| [PivotSource](#pivotsource) | String | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "Pivo |
| [PlotBy](#plotby) | int | Gets and sets whether plot by row or column. The value of the property is PlotDataByType integer constant. |
| [PlotEmptyCellsType](#plotemptycellstype) | int | Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [PlotVisibleCells](#plotvisiblecells) | boolean | Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly p |
| [PlotVisibleCellsOnly](#plotvisiblecellsonly) | boolean | Indicates whether plot visible cells only. |
| [DisplayNaAsBlank](#displaynaasblank) | boolean | Indicates whether displaying #N/A as blank value. |
| [Name](#name) | String | Gets and sets the name of the chart. |
| [SizeWithWindow](#sizewithwindow) | boolean | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [Worksheet](#worksheet) | Worksheet | Gets the worksheet which contains this chart. |
| [Shapes](#shapes) | ShapeCollection | Returns all drawing shapes in this chart. |
| [PrintSize](#printsize) | int | Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant. |
| [Type](#type) | int | Gets or sets a chart's type. The value of the property is ChartType integer constant. |
| [NSeries](#nseries) | SeriesCollection | Gets a SeriesCollection collection representing the data series in the chart. |
| [FilteredNSeries](#filterednseries) | SeriesCollection | Gets a SeriesCollection collection representing the data series that are filtered in the chart. |
| [Title](#title) | Title | Gets the chart's title. |
| [SubTitle](#subtitle) | Title | Gets the chart's sub-title. Only for ODS format file. |
| [PlotArea](#plotarea) | PlotArea | Gets the chart's plot area which includes axis tick labels. |
| [ChartArea](#chartarea) | ChartArea | Gets the chart area in the worksheet. |
| [CategoryAxis](#categoryaxis) | Axis | Gets the chart's X axis. |
| [ValueAxis](#valueaxis) | Axis | Gets the chart's Y axis. |
| [SecondValueAxis](#secondvalueaxis) | Axis | Gets the chart's second Y axis. |
| [SecondCategoryAxis](#secondcategoryaxis) | Axis | Gets the chart's second X axis. |
| [SeriesAxis](#seriesaxis) | Axis | Gets the chart's series axis. |
| [Legend](#legend) | Legend | Gets the chart legend. |
| [ChartDataTable](#chartdatatable) | ChartDataTable | Represents the chart data table. |
| [ShowLegend](#showlegend) | boolean | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [IsRectangularCornered](#isrectangularcornered) | boolean | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [ShowDataTable](#showdatatable) | boolean | Gets or sets a value indicating whether the chart displays a data table. |
| [FirstSliceAngle](#firstsliceangle) | int | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [GapWidth](#gapwidth) | int | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [GapDepth](#gapdepth) | int | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this |
| [Floor](#floor) | Floor | Returns a Floor object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts. |
| [Walls](#walls) | Walls | Returns a Walls object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts. |
| [BackWall](#backwall) | Walls | Returns a Walls object that represents the back wall of a 3-D chart. |
| [SideWall](#sidewall) | Walls | Returns a Walls object that represents the side wall of a 3-D chart. |
| [WallsAndGridlines2D](#wallsandgridlines2d) | boolean | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [RotationAngle](#rotationangle) | int | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value o |
| [Elevation](#elevation) | int | Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the char |
| [RightAngleAxes](#rightangleaxes) | boolean | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this pro |
| [AutoScaling](#autoscaling) | boolean | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes p |
| [HeightPercent](#heightpercent) | int | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [Perspective](#perspective) | int | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the Right |
| [Is3D](#is3d) | boolean | Indicates whether the chart is a 3d chart. |
| [DepthPercent](#depthpercent) | int | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [ActualChartSize](#actualchartsize) | int[] | Gets actual size of chart in unit of pixels. NOTE: This member is now obsolete. Instead, please use Chart.getActualSize( |
| [Placement](#placement) | int | Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer const |
| [PageSetup](#pagesetup) | PageSetup | Represents the page setup description in this chart. |
| [ChartShape](#chartshape) | ChartShape | Represents the chartShape; NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Chart.ChartObject  |
| [Line](#line) | Line | Gets the line. |

## Methods

| Name | Description |
| --- | --- |
| [toImage](#toimage) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.

The  |
| [toPdf](#topdf) | Saves the chart to a pdf file. |
| [getActualSize](#getactualsize) | Gets actual size of chart in unit of pixels. |
| [hasAxis](#hasaxis) | Returns which axes exist on the chart.

Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, Doughn |
| [switchRowColumn](#switchrowcolumn) | Switches row/column. |
| [getChartDataRange](#getchartdatarange) | Gets the data source range of the chart.

Only supports range. |
| [setChartDataRange](#setchartdatarange) | Specifies data range for a chart. |
| [isReferedByChart](#isreferedbychart) | Returns whether the cell refered by the chart.

NOTE: This method is now obsolete. Instead, please use IsCellReferedByCh |
| [isCellReferedByChart](#iscellreferedbychart) | Returns whether the cell refered by the chart. |
| [isChartDataChanged](#ischartdatachanged) | Detects if a chart's data source has changed.

The method detects the changes in the chart's data source before renderin |
| [refreshPivotData](#refreshpivotdata) | Refreshes chart's data from pivot table.

We will gather data from pivot data source to the pivot table report. This met |
| [changeTemplate](#changetemplate) | Change chart type with preset template. |
| [move](#move) | Moves the chart to a specified location. |
| [calculate](#calculate) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [toImageBytes](#toimagebytes) | Creates the chart image and saves it to a byte array in the specified format.

The format of the image is specified by u |
| [toPdfBytes](#topdfbytes) | Creates the chart pdf and saves it to a byte array. |

### Chart.Style property {#style}

Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set.

**Type:** int

### Chart.ChartObject property {#chartobject}

Represents the chartShape;

**Type:** ChartShape

### Chart.HidePivotFieldButtons property {#hidepivotfieldbuttons}

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

**Type:** boolean

### Chart.PivotOptions property {#pivotoptions}

Specifies the pivot controls that appear on the chart

**Type:** PivotOptions

### Chart.PivotSource property {#pivotsource}

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

**Type:** String

### Chart.PlotBy property {#plotby}

Gets and sets whether plot by row or column. The value of the property is PlotDataByType integer constant.

**Type:** int

### Chart.PlotEmptyCellsType property {#plotemptycellstype}

Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant.

**Type:** int

### Chart.PlotVisibleCells property {#plotvisiblecells}

Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### Chart.PlotVisibleCellsOnly property {#plotvisiblecellsonly}

Indicates whether plot visible cells only.

**Type:** boolean

### Chart.DisplayNaAsBlank property {#displaynaasblank}

Indicates whether displaying #N/A as blank value.

**Type:** boolean

### Chart.Name property {#name}

Gets and sets the name of the chart.

**Type:** String

### Chart.SizeWithWindow property {#sizewithwindow}

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

**Type:** boolean

### Chart.Worksheet property {#worksheet}

Gets the worksheet which contains this chart.

**Type:** Worksheet

### Chart.Shapes property {#shapes}

Returns all drawing shapes in this chart.

**Type:** ShapeCollection

### Chart.PrintSize property {#printsize}

Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant.

**Type:** int

### Chart.Type property {#type}

Gets or sets a chart's type. The value of the property is ChartType integer constant.

**Type:** int

### Chart.NSeries property {#nseries}

Gets a SeriesCollection collection representing the data series in the chart.

**Type:** SeriesCollection

### Chart.FilteredNSeries property {#filterednseries}

Gets a SeriesCollection collection representing the data series that are filtered in the chart.

**Type:** SeriesCollection

### Chart.Title property {#title}

Gets the chart's title.

**Type:** Title

### Chart.SubTitle property {#subtitle}

Gets the chart's sub-title. Only for ODS format file.

**Type:** Title

### Chart.PlotArea property {#plotarea}

Gets the chart's plot area which includes axis tick labels.

**Type:** PlotArea

### Chart.ChartArea property {#chartarea}

Gets the chart area in the worksheet.

**Type:** ChartArea

### Chart.CategoryAxis property {#categoryaxis}

Gets the chart's X axis.

**Type:** Axis

### Chart.ValueAxis property {#valueaxis}

Gets the chart's Y axis.

**Type:** Axis

### Chart.SecondValueAxis property {#secondvalueaxis}

Gets the chart's second Y axis.

**Type:** Axis

### Chart.SecondCategoryAxis property {#secondcategoryaxis}

Gets the chart's second X axis.

**Type:** Axis

### Chart.SeriesAxis property {#seriesaxis}

Gets the chart's series axis.

**Type:** Axis

### Chart.Legend property {#legend}

Gets the chart legend.

**Type:** Legend

### Chart.ChartDataTable property {#chartdatatable}

Represents the chart data table.

**Type:** ChartDataTable

### Chart.ShowLegend property {#showlegend}

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

**Type:** boolean

### Chart.IsRectangularCornered property {#isrectangularcornered}

Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.

**Type:** boolean

### Chart.ShowDataTable property {#showdatatable}

Gets or sets a value indicating whether the chart displays a data table.

**Type:** boolean

### Chart.FirstSliceAngle property {#firstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

**Type:** int

### Chart.GapWidth property {#gapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

**Type:** int

### Chart.GapDepth property {#gapdepth}

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

**Type:** int

### Chart.Floor property {#floor}

Returns a Floor object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts.

**Type:** Floor

### Chart.Walls property {#walls}

Returns a Walls object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts.

**Type:** Walls

### Chart.BackWall property {#backwall}

Returns a Walls object that represents the back wall of a 3-D chart.

**Type:** Walls

### Chart.SideWall property {#sidewall}

Returns a Walls object that represents the side wall of a 3-D chart.

**Type:** Walls

### Chart.WallsAndGridlines2D property {#wallsandgridlines2d}

True if gridlines are drawn two-dimensionally on a 3-D chart.

**Type:** boolean

### Chart.RotationAngle property {#rotationangle}

Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.

**Type:** int

### Chart.Elevation property {#elevation}

Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

**Type:** int

### Chart.RightAngleAxes property {#rightangleaxes}

True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this property is True, the Perspective property is ignored.

**Type:** boolean

### Chart.AutoScaling property {#autoscaling}

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

**Type:** boolean

### Chart.HeightPercent property {#heightpercent}

Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).

**Type:** int

### Chart.Perspective property {#perspective}

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

**Type:** int

### Chart.Is3D property {#is3d}

Indicates whether the chart is a 3d chart.

**Type:** boolean

### Chart.DepthPercent property {#depthpercent}

Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).

**Type:** int

### Chart.ActualChartSize property {#actualchartsize}

Gets actual size of chart in unit of pixels. NOTE: This member is now obsolete. Instead, please use Chart.getActualSize() method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int[]

### Chart.Placement property {#placement}

Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer constant.

**Type:** int

### Chart.PageSetup property {#pagesetup}

Represents the page setup description in this chart.

**Type:** PageSetup

### Chart.ChartShape property {#chartshape}

Represents the chartShape; NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Chart.ChartObject property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** ChartShape

### Chart.Line property {#line}

Gets the line.

**Type:** Line

### toImage(imageFile) (1 of 5) {#toimage}

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.

The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |

---

### toImage(imageFile, imageFormat) (2 of 5) {#toimage-1}

Creates the chart image and saves it to a file in the specified format.

NOTE: This member is now obsolete. Instead, please use Chart.ToImage(string, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageFormat | ImageFormat | The format in which to save the image. |

---

### toImage(imageFile, imageType) (3 of 5) {#toimage-2}

Creates the chart image and saves it to a file in the specified image type.

The type of the image is specified by using imageType . The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageType | int | A ImageType value. The image type in which to save the image. |

---

### toImage(imageFile, jpegQuality) (4 of 5) {#toimage-3}

Creates the chart image and saves it to a file in the Jpeg format.

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| jpegQuality | long | Jpeg quality. |

---

### toImage(imageFile, options) (5 of 5) {#toimage-4}

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.

The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| options | ImageOrPrintOptions | Additional image creation options |

**Example:**

```python
options = ImageOrPrintOptions()
options.setHorizontalResolution(300)
options.setVerticalResolution(300)

book = Workbook("Book2.xlsx")
book.getWorksheets().get(3).getCharts().get(0).toImage("chart.png", options)
```

### toPdf(fileName) (1 of 2) {#topdf}

Saves the chart to a pdf file.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |

---

### toPdf(fileName, desiredPageWidth, desiredPageHeight, hAlignmentType, vAlignmentType) (2 of 2) {#topdf-1}

Saves the chart to a pdf file.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |
| desiredPageWidth | float | The desired page width in inches. |
| desiredPageHeight | float | The desired page height in inches. |
| hAlignmentType | int | A PageLayoutAlignmentType value. The chart horizontal alignment type in the output page. |
| vAlignmentType | int | A PageLayoutAlignmentType value. The chart vertical alignment type in the output page. |

### getActualSize() {#getactualsize}

Gets actual size of chart in unit of pixels.

**Returns:** Actual size in an array(width and height). [0] is width; [1] is height.

### hasAxis(aixsType, isPrimary) {#hasaxis}

Returns which axes exist on the chart.

Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.

### switchRowColumn() {#switchrowcolumn}

Switches row/column.

**Returns:** False means switching row/column fails.

### getChartDataRange() {#getchartdatarange}

Gets the data source range of the chart.

Only supports range.

**Returns:** The data source.

### setChartDataRange(area, isVertical) {#setchartdatarange}

Specifies data range for a chart.

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### isReferedByChart(rowIndex, columnIndex) {#isreferedbychart}

Returns whether the cell refered by the chart.

NOTE: This method is now obsolete. Instead, please use IsCellReferedByChart(int,int,int) method. This method will be removed 12 months later since April 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The row index |
| columnIndex | int | The column index |

### isCellReferedByChart(sheetIndex, rowIndex, columnIndex) {#iscellreferedbychart}

Returns whether the cell refered by the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | int | The row index |
| columnIndex | int | The column index |

### isChartDataChanged() {#ischartdatachanged}

Detects if a chart's data source has changed.

The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.

**Returns:** Returns true if the chart has changed otherwise returns false

### refreshPivotData() {#refreshpivotdata}

Refreshes chart's data from pivot table.

We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.

### changeTemplate(data) {#changetemplate}

Change chart type with preset template.

| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The data of chart template file(.crtx). |

### move(topRow, leftColumn, bottomRow, rightColumn) {#move}

Moves the chart to a specified location.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftColumn |  | Upper left column index. |
| upperLeftRow |  | Upper left row index. |
| lowerRightColumn |  | Lower right column index |
| lowerRightRow |  | Lower right row index |

### calculate() (1 of 2) {#calculate}

Calculates the custom position of plot area, axes if the position of them are auto assigned.

---

### calculate(calculateOptions) (2 of 2) {#calculate-1}

Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.

### toImageBytes(options) {#toimagebytes}

Creates the chart image and saves it to a byte array in the specified format.

The format of the image is specified by using options.ImageFormat . The following formats are supported: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Addtional image creation options |

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("Book2.xlsx")
imgOptions = ImageOrPrintOptions()
imgOptions.setHorizontalResolution(200)
imgOptions.setVerticalResolution(300)
imgOptions.setImageFormat(ImageFormat.getJpeg())
chart = wb.getWorksheets().get("Chart").getCharts().get(0)
with open("chart.jpeg", "wb") as w:
    content = chart.toImageBytes(imgOptions)
    w.write(content)

jpype.shutdownJVM()
```

### toPdfBytes() (1 of 2) {#topdfbytes}

Creates the chart pdf and saves it to a byte array.

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("Book2.xlsx")
chart = wb.getWorksheets().get("Chart").getCharts().get(0)
with open("chart.pdf", "wb") as w:
    content = chart.toPdfBytes()
    w.write(content)

jpype.shutdownJVM()
```

---

### toPdfBytes(desiredPageWidth, desiredPageHeight, hAlignmentType, vAlignmentType) (2 of 2) {#topdfbytes-1}

Creates the chart pdf and saves it to a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredPageWidth | float | The desired page width in inches |
| desiredPageHeight | float | The desired page height in inches |
| hAlignmentType | int | A PageLayoutAlignmentType value. The chart horizontal alignment type in the output page |
| vAlignmentType | int | A PageLayoutAlignmentType value. The chart vertical alignment type in the output page |

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("Book2.xlsx")
chart = wb.getWorksheets().get("Chart").getCharts().get(0)
with open("chart2.pdf", "wb") as w:
    content = chart.toPdfBytes(80, 60, PageLayoutAlignmentType.LEFT, PageLayoutAlignmentType.TOP)
    w.write(content)

jpype.shutdownJVM()
```
