##Floor
Encapsulates the object that represents the floor of a 3-D chart.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area)
```
public class Floor extends Area
```
Encapsulates the object that represents the floor of a 3-D chart.
**Example**
```
//Instantiate the License class
License license = new License();
//Pass only the name of the license file embedded in the assembly
license.setLicense("Aspose.Cells.lic");
//Instantiate the workbook object
Workbook workbook = new Workbook();
//Get cells collection
Cells cells = workbook.getWorksheets().get(0).getCells();
//Put values in cells
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
cells.get("A3").putValue(3);
//get charts colletion
ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
//add a new chart
int index = charts.add(ChartType.COLUMN_3_D_STACKED, 5, 0, 15, 5);
//get the newly added chart
Chart chart = charts.get(index);
//set charts nseries
chart.getNSeries().add("A1:A3", true);
//Show data labels
chart.getNSeries().get(0).getDataLabels().setShowValue(true);
//Get chart's floor
Floor floor = chart.getFloor();
//set floor's border as red
floor.getBorder().setColor(com.aspose.cells.Color.getRed());
//set fill format
floor.getFillFormat().setPresetColorGradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2);
//save the file
workbook.save("dest.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Gets the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | Gets the border [Line](../../com.aspose.cells/line). |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | Represents a [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified chart or shape. |
| [getForegroundColor()](#getForegroundColor--) | Gets the foreground [Color](../../com.aspose.cells/color). |
| [getFormatting()](#getFormatting--) | Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
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
