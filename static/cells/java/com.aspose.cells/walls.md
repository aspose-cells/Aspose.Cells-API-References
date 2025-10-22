##Walls
Encapsulates the object that represents the walls of a 3-D chart.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area), [com.aspose.cells.Floor](../../com.aspose.cells/floor)
```
public class Walls extends Floor
```
Encapsulates the object that represents the walls of a 3-D chart.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Gets the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | Gets the border [Line](../../com.aspose.cells/line). |
| [getCenterX()](#getCenterX--) | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getCenterXPx()](#getCenterXPx--) | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getCenterY()](#getCenterY--) | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getCenterYPx()](#getCenterYPx--) | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getClass()](#getClass--) |  |
| [getCubePointCount()](#getCubePointCount--) | Gets the number of cube points after calls Chart.Calculate() method. |
| [getCubePointXPx(int index)](#getCubePointXPx-int-) | Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. |
| [getCubePointYPx(int index)](#getCubePointYPx-int-) | Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. |
| [getDepth()](#getDepth--) | Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getDepthPx()](#getDepthPx--) | Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [getFillFormat()](#getFillFormat--) | Represents a [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified chart or shape. |
| [getForegroundColor()](#getForegroundColor--) | Gets the foreground [Color](../../com.aspose.cells/color). |
| [getFormatting()](#getFormatting--) | Represents the formatting of the area. |
| [getHeight()](#getHeight--) | Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getHeightPx()](#getHeightPx--) | Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [getInvertIfNegative()](#getInvertIfNegative--) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getWidth()](#getWidth--) | Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getWidthPx()](#getWidthPx--) | Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Sets the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area). |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | Sets the border [Line](../../com.aspose.cells/line). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Sets the foreground [Color](../../com.aspose.cells/color). |
| [setFormatting(int value)](#setFormatting-int-) | Represents the formatting of the area. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setTransparency(double value)](#setTransparency-double-) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
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
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```
Gets the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area).
**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```
Gets the border [Line](../../com.aspose.cells/line).
**Returns:**
[Line](../../com.aspose.cells/line)
### getCenterX() {#getCenterX--}
```
public int getCenterX()
```
Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method.
**Returns:**
int
### getCenterXPx() {#getCenterXPx--}
```
public int getCenterXPx()
```
Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getCenterY() {#getCenterY--}
```
public int getCenterY()
```
Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method.
**Returns:**
int
### getCenterYPx() {#getCenterYPx--}
```
public int getCenterYPx()
```
Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCubePointCount() {#getCubePointCount--}
```
public int getCubePointCount()
```
Gets the number of cube points after calls Chart.Calculate() method.
**Returns:**
int
### getCubePointXPx(int index) {#getCubePointXPx-int-}
```
public float getCubePointXPx(int index)
```
Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getCubePointYPx(int index) {#getCubePointYPx-int-}
```
public float getCubePointYPx(int index)
```
Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
float
### getDepth() {#getDepth--}
```
public int getDepth()
```
Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method.
**Returns:**
int
### getDepthPx() {#getDepthPx--}
```
public int getDepthPx()
```
Gets the depth front to back in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getFillFormat() {#getFillFormat--}
```
public FillFormat getFillFormat()
```
Represents a [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified chart or shape.
**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```
Gets the foreground [Color](../../com.aspose.cells/color).
**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```
Represents the formatting of the area.
See [FormattingType](../../com.aspose.cells/formattingtype).
**Returns:**
int
### getHeight() {#getHeight--}
```
public int getHeight()
```
Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method.
**Returns:**
int
### getHeightPx() {#getHeightPx--}
```
public int getHeightPx()
```
Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(-100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a chart to the worksheet
int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.getNSeries().add("A1:A3", true);
chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
//Setting the foreground color of the 1st NSeries area
chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
//Setting the background color of the 1st NSeries area.
//The displayed area color of second chart point will be the background color.
chart.getNSeries().get(0).getArea().setBackgroundColor(Color.getYellow());
//Saving the Excel file
workbook.save("book1.xls");
```
**Returns:**
boolean
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
**Returns:**
double
### getWidth() {#getWidth--}
```
public int getWidth()
```
Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method.
**Returns:**
int
### getWidthPx() {#getWidthPx--}
```
public int getWidthPx()
```
Gets the width of left to right in units of pixels after calls Chart.Calculate() method.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```
Sets the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```
Sets the border [Line](../../com.aspose.cells/line).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |
### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```
Sets the foreground [Color](../../com.aspose.cells/color).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```
Represents the formatting of the area.
See [FormattingType](../../com.aspose.cells/formattingtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
