##ChartPoint
Represents a single point in a series in a chart.
**Inheritance:**
java.lang.Object
```
public class ChartPoint
```
Represents a single point in a series in a chart.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a chart to the worksheet
int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
Chart chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.getNSeries().add("A1:B3", true);
//Show Data Labels
chart.getNSeries().get(0).getDataLabels().setShowValue(true);
for (int i = 0; i  <chart.getNSeries().get(0).getPoints().getCount(); i++)
{
//Get Data Point
ChartPoint point = chart.getNSeries().get(0).getPoints().get(i);
//Set Pir Explosion
point.setExplosion(15);
//Set Border Color
point.getBorder().setColor(com.aspose.cells.Color.getRed());
}
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. |
| [getArea()](#getArea--) | Gets the [Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | Gets the [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [getBottomPointCount()](#getBottomPointCount--) | Gets the number of bottom points after calls Chart.Calculate() method. |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Returns a [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) object that represents the data label associated with this chart point. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. |
| [getEndAngle()](#getEndAngle--) | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. |
| [getExplosion()](#getExplosion--) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. |
| [getMarker()](#getMarker--) | Gets the [Series.getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Gets the number of the points on category axis after calls Chart.Calculate() method. |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. |
| [getRadiusPx()](#getRadiusPx--) | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [getShadow()](#getShadow--) | True if the chartpoint has a shadow. |
| [getShapeHeight()](#getShapeHeight--) | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeHeightPx()](#getShapeHeightPx--) | Gets the height in units of pixels after calls Chart.Calculate() method. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) object that holds the visual shape properties of the ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeWidthPx()](#getShapeWidthPx--) | Gets the width in units of pixels after calls Chart.Calculate() method. |
| [getShapeX()](#getShapeX--) | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeXPx()](#getShapeXPx--) | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeY()](#getShapeY--) | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeYPx()](#getShapeYPx--) | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getStartAngle()](#getStartAngle--) | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. |
| [getTopPointCount()](#getTopPointCount--) | Gets the number of top points after calls Chart.Calculate() method. |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. |
| [getXValue()](#getXValue--) | Gets the X value of the chart point. |
| [getXValueType()](#getXValueType--) | Gets X value type of the chart point. |
| [getYValue()](#getYValue--) | Gets the Y value of the chart point. |
| [getYValueType()](#getYValueType--) | Gets Y value type of the chart point. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Gets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the chartpoint has a shadow. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Sets the X value of the chart point. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Sets the Y value of the chart point. |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```
Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```
Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```
Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```
Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```
Gets the [Area](../../com.aspose.cells/area).
**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```
Gets the [Line](../../com.aspose.cells/line).
**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```
Gets the width of border in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```
Gets the number of bottom points after calls Chart.Calculate() method.
**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```
Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```
Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```
Returns a [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) object that represents the data label associated with this chart point.
**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```
Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```
Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```
The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.
**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```
Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```
Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```
Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```
Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```
Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```
Gets the [Series.getMarker()](../../com.aspose.cells/series\#getMarker--).
**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```
Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.
**Remarks**
Area 2D chart return 1 Area 3D chart return 2.
**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```
Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.
**Remarks**
Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```
Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.
**Remarks**
Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```
Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```
True if the chartpoint has a shadow.
**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```
Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.
**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```
Gets the height in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```
Gets the [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) object that holds the visual shape properties of the ChartPoint.
**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```
Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.
**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```
Gets the width in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```
Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.
**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```
Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```
Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.
**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```
Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```
Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```
Gets the number of top points after calls Chart.Calculate() method.
**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```
Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```
Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```
Gets the X value of the chart point.
**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```
Gets X value type of the chart point.
See [CellValueType](../../com.aspose.cells/cellvaluetype).
**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```
Gets the Y value of the chart point.
**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```
Gets Y value type of the chart point.
See [CellValueType](../../com.aspose.cells/cellvaluetype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isInSecondaryPlot() {#isInSecondaryPlot--}
```
public boolean isInSecondaryPlot()
```
Gets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```
The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```
Sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```
True if the chartpoint has a shadow.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```
Sets the X value of the chart point.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```
Sets the Y value of the chart point.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
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
