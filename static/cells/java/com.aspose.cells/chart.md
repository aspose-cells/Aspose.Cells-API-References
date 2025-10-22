##Chart
Encapsulates the object that represents a single Excel chart.
**Inheritance:**
java.lang.Object
```
public class Chart
```
Encapsulates the object that represents a single Excel chart.
**Example**
The following codes show how to create a chart with .Net codes.
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
## Methods
| Method | Description |
| --- | --- |
| [calculate()](#calculate--) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Change chart type with preset template. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Gets actual size of chart in unit of pixels. |
| [getActualSize()](#getActualSize--) | Gets actual size of chart in unit of pixels. |
| [getAutoScaling()](#getAutoScaling--) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. |
| [getBackWall()](#getBackWall--) | Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the back wall of a 3-D chart. |
| [getCategoryAxis()](#getCategoryAxis--) | Gets the chart's X axis. |
| [getChartArea()](#getChartArea--) | Gets the chart area in the worksheet. |
| [getChartDataRange()](#getChartDataRange--) | Gets the data source range of the chart. |
| [getChartDataTable()](#getChartDataTable--) | Represents the chart data table. |
| [getChartObject()](#getChartObject--) | Represents the chartShape; |
| [getChartShape()](#getChartShape--) | Represents the chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Indicates whether displaying \#N/A as blank value. |
| [getElevation()](#getElevation--) | Represents the elevation of the 3-D chart view, in degrees. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Gets a [SeriesCollection](../../com.aspose.cells/seriescollection) collection representing the data series that are filtered in the chart. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Gets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). |
| [getFloor()](#getFloor--) | Returns a [getFloor()](../../com.aspose.cells/chart\#getFloor--) object that represents the walls of a 3-D chart. |
| [getGapDepth()](#getGapDepth--) | Gets the distance between the data series in a 3-D chart, as a percentage of the marker width. |
| [getGapWidth()](#getGapWidth--) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. |
| [getHeightPercent()](#getHeightPercent--) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [getIs3D()](#getIs3D--) | Indicates whether the chart is a 3d chart. |
| [getLegend()](#getLegend--) | Gets the chart legend. |
| [getLine()](#getLine--) | Gets the line. |
| [getNSeries()](#getNSeries--) | Gets a [SeriesCollection](../../com.aspose.cells/seriescollection) collection representing the data series in the chart. |
| [getName()](#getName--) | Gets the name of the chart. |
| [getPageSetup()](#getPageSetup--) | Represents the page setup description in this chart. |
| [getPerspective()](#getPerspective--) | Returns or sets the perspective for the 3-D chart view. |
| [getPivotOptions()](#getPivotOptions--) | Specifies the pivot controls that appear on the chart |
| [getPivotSource()](#getPivotSource--) | The source is the data of the pivotTable. |
| [getPlacement()](#getPlacement--) | Represents the way the chart is attached to the cells below it. |
| [getPlotArea()](#getPlotArea--) | Gets the chart's plot area which includes axis tick labels. |
| [getPlotBy()](#getPlotBy--) | Gets whether plot by row or column. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Gets how to plot the empty cells. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Indicates whether only plot visible cells. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Indicates whether plot visible cells only. |
| [getPrintSize()](#getPrintSize--) | Gets the printed chart size. |
| [getRightAngleAxes()](#getRightAngleAxes--) | True if the chart axes are at right angles. |
| [getRotationAngle()](#getRotationAngle--) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Gets the chart's second X axis. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Gets the chart's second Y axis. |
| [getSeriesAxis()](#getSeriesAxis--) | Gets the chart's series axis. |
| [getShapes()](#getShapes--) | Returns all drawing shapes in this chart. |
| [getShowDataTable()](#getShowDataTable--) | Gets a value indicating whether the chart displays a data table. |
| [getShowLegend()](#getShowLegend--) | Gets a value indicating whether the chart legend will be displayed. |
| [getSideWall()](#getSideWall--) | Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the side wall of a 3-D chart. |
| [getSizeWithWindow()](#getSizeWithWindow--) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [getStyle()](#getStyle--) | Gets the builtin style. |
| [getSubTitle()](#getSubTitle--) | Gets the chart's sub-title. |
| [getTitle()](#getTitle--) | Gets the chart's title. |
| [getType()](#getType--) | Gets a chart's type. |
| [getValueAxis()](#getValueAxis--) | Gets the chart's Y axis. |
| [getWalls()](#getWalls--) | Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the walls of a 3-D chart. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [getWorksheet()](#getWorksheet--) | Gets the worksheet which contains this chart. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Returns which axes exist on the chart. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Returns whether the cell refered by the chart. |
| [isChartDataChanged()](#isChartDataChanged--) | Detects if a chart's data source has changed. |
| [isRectangularCornered()](#isRectangularCornered--) | Gets a value indicating whether the chart area is rectangular cornered. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Returns whether the cell refered by the chart. |
| [move(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#move-int-int-int-int-) | Moves the chart to a specified location. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Refreshes chart's data from pivot table. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Specifies data range for a chart. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Indicates whether displaying \#N/A as blank value. |
| [setElevation(int value)](#setElevation-int-) | Represents the elevation of the 3-D chart view, in degrees. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). |
| [setGapDepth(int value)](#setGapDepth-int-) | Sets the distance between the data series in a 3-D chart, as a percentage of the marker width. |
| [setGapWidth(int value)](#setGapWidth-int-) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the chart. |
| [setPerspective(short value)](#setPerspective-short-) | Returns or sets the perspective for the 3-D chart view. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | The source is the data of the pivotTable. |
| [setPlacement(int value)](#setPlacement-int-) | Represents the way the chart is attached to the cells below it. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Sets how to plot the empty cells. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Indicates whether only plot visible cells. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Indicates whether plot visible cells only. |
| [setPrintSize(int value)](#setPrintSize-int-) | Sets the printed chart size. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Sets a value indicating whether the chart area is rectangular cornered. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | True if the chart axes are at right angles. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Sets a value indicating whether the chart displays a data table. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Sets a value indicating whether the chart legend will be displayed. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [setStyle(int value)](#setStyle-int-) | Sets the builtin style. |
| [setType(int value)](#setType-int-) | Sets a chart's type. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [switchRowColumn()](#switchRowColumn--) | Switches row/column. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Creates the chart image and saves it to a stream in the specified format. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Creates the chart image and saves it to a file. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Creates the chart image and saves it to a file in the specified format. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Creates the chart image and saves it to a file. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Creates the chart image and saves it to a file in the specified image type. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Creates the chart image and saves it to a file in the Jpeg format. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Creates the chart pdf and saves it to a stream. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Creates the chart pdf and saves it to a stream. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Saves the chart to a pdf file. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Saves the chart to a pdf file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```
Calculates the custom position of plot area, axes if the position of them are auto assigned.
### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```
Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |
### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```
Change chart type with preset template.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The data of chart template file(.crtx). |
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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```
Gets actual size of chart in unit of pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Chart.getActualSize() method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int[] - Actual size in an array(width and height). [0] is width; [1] is height.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```
Gets actual size of chart in unit of pixels.
**Returns:**
int[] - Actual size in an array(width and height). [0] is width; [1] is height.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```
True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.
**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```
Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the back wall of a 3-D chart.
**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```
Gets the chart's X axis.
**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```
Gets the chart area in the worksheet.
**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```
Gets the data source range of the chart.
**Remarks**
Only supports range.
**Returns:**
java.lang.String - The data source.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```
Represents the chart data table.
**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```
Represents the chartShape;
**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```
Represents the chartShape;
**Remarks**
NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Chart.ChartObject property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.
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
Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).
**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```
Indicates whether displaying \#N/A as blank value.
**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```
Represents the elevation of the 3-D chart view, in degrees.
**Remarks**
The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.
**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```
Gets a [SeriesCollection](../../com.aspose.cells/seriescollection) collection representing the data series that are filtered in the chart.
**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```
Gets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.
**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```
Returns a [getFloor()](../../com.aspose.cells/chart\#getFloor--) object that represents the walls of a 3-D chart.
**Remarks**
This property doesn't apply to 3-D pie charts.
**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```
Gets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.
**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```
Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.
**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```
Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).
**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```
Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.
**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```
Indicates whether the chart is a 3d chart.
**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```
Gets the chart legend.
**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```
Gets the line.
**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```
Gets a [SeriesCollection](../../com.aspose.cells/seriescollection) collection representing the data series in the chart.
**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```
Gets the name of the chart.
**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```
Represents the page setup description in this chart.
**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```
Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.
**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```
Specifies the pivot controls that appear on the chart
**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```
The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.
**Remarks**
If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.
**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```
Represents the way the chart is attached to the cells below it.
See [PlacementType](../../com.aspose.cells/placementtype).
**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```
Gets the chart's plot area which includes axis tick labels.
**Remarks**
**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```
Gets whether plot by row or column.
See [PlotDataByType](../../com.aspose.cells/plotdatabytype).
**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```
Gets how to plot the empty cells.
See [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).
**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```
Indicates whether only plot visible cells.
**Remarks**
NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```
Indicates whether plot visible cells only.
**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```
Gets the printed chart size.
See [PrintSizeType](../../com.aspose.cells/printsizetype).
**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```
True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).
**Remarks**
If this property is True, the Perspective property is ignored.
**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```
Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).
**Remarks**
The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.
**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```
Gets the chart's second X axis.
**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```
Gets the chart's second Y axis.
**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```
Gets the chart's series axis.
**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```
Returns all drawing shapes in this chart.
**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```
Gets a value indicating whether the chart displays a data table.
**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```
Gets a value indicating whether the chart legend will be displayed. Default is true.
**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```
Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the side wall of a 3-D chart.
**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```
True if Microsoft Excel resizes the chart to match the size of the chart sheet window.
**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```
Gets the builtin style.
**Remarks**
It should be between 1 and 48. Return -1 if it's not be set.
**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```
Gets the chart's sub-title. Only for ODS format file.
**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```
Gets the chart's title.
**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```
Gets a chart's type.
See [ChartType](../../com.aspose.cells/charttype).
**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```
Gets the chart's Y axis.
**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```
Returns a [getWalls()](../../com.aspose.cells/chart\#getWalls--) object that represents the walls of a 3-D chart.
**Remarks**
This property doesn't apply to 3-D pie charts.
**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```
True if gridlines are drawn two-dimensionally on a 3-D chart.
**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```
Gets the worksheet which contains this chart.
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```
Returns which axes exist on the chart.
**Remarks**
Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.
**Parameters:**
| Parameter | Type | Description |
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
Returns whether the cell refered by the chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | int | The row index |
| columnIndex | int | The column index |
**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```
Detects if a chart's data source has changed.
**Remarks**
The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.
**Returns:**
boolean - Returns true if the chart has changed otherwise returns false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```
Gets a value indicating whether the chart area is rectangular cornered. Default is true.
**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```
Returns whether the cell refered by the chart.
**Remarks**
NOTE: This method is now obsolete. Instead, please use IsCellReferedByChart(int,int,int) method. This method will be removed 12 months later since April 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int | The row index |
| columnIndex | int | The column index |
**Returns:**
boolean -
### move(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#move-int-int-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```
Moves the chart to a specified location.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |
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
Refreshes chart's data from pivot table.
**Remarks**
We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.
### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```
True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```
Specifies data range for a chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```
Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```
Indicates whether displaying \#N/A as blank value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```
Represents the elevation of the 3-D chart view, in degrees.
**Remarks**
The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```
Sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```
Sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```
Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```
Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```
Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```
Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |
### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```
The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.
**Remarks**
If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```
Represents the way the chart is attached to the cells below it.
See [PlacementType](../../com.aspose.cells/placementtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```
Sets how to plot the empty cells.
See [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```
Indicates whether only plot visible cells.
**Remarks**
NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```
Indicates whether plot visible cells only.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```
Sets the printed chart size.
See [PrintSizeType](../../com.aspose.cells/printsizetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```
Sets a value indicating whether the chart area is rectangular cornered. Default is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```
True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).
**Remarks**
If this property is True, the Perspective property is ignored.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```
Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).
**Remarks**
The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```
Sets a value indicating whether the chart displays a data table.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```
Sets a value indicating whether the chart legend will be displayed. Default is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```
True if Microsoft Excel resizes the chart to match the size of the chart sheet window.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```
Sets the builtin style.
**Remarks**
It should be between 1 and 48. Return -1 if it's not be set.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Sets a chart's type.
See [ChartType](../../com.aspose.cells/charttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```
True if gridlines are drawn two-dimensionally on a 3-D chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```
Switches row/column.
**Returns:**
boolean - False means switching row/column fails.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```
Creates the chart image and saves it to a stream in the specified format.
**Remarks**
The format of the image is specified by using `options.ImageFormat`. The following formats are supported: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List][] for more details.
[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The output stream. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Additional image creation options |
### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | The image file name with full path. |
### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```
Creates the chart image and saves it to a file in the specified format.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Chart.ToImage(string, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | The image file name with full path. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | The format in which to save the image. |
### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List][] for more details.
**Example**
Saves to Tiff with 300 dpi and CCITT4 compression.
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
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | The image file name with full path. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Additional image creation options |
### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```
Creates the chart image and saves it to a file in the specified image type.
**Remarks**
The type of the image is specified by using `imageType`. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | The image file name with full path. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). The image type in which to save the image. |
### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```
Creates the chart image and saves it to a file in the Jpeg format.
**Remarks**
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String | The image file name with full path. |
| jpegQuality | long | Jpeg quality. |
### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```
Creates the chart pdf and saves it to a stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The output stream. |
### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```
Creates the chart pdf and saves it to a stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The output stream. |
| desiredPageWidth | float | The desired page width in inches. |
| desiredPageHeight | float | The desired page height in inches. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). The chart horizontal alignment type in the output page. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). The chart vertical alignment type in the output page. |
### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```
Saves the chart to a pdf file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the pdf file name with full path |
### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```
Saves the chart to a pdf file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the pdf file name with full path |
| desiredPageWidth | float | The desired page width in inches. |
| desiredPageHeight | float | The desired page height in inches. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). The chart horizontal alignment type in the output page. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). The chart vertical alignment type in the output page. |
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
