##ChartPointCollection
Represents a collection that contains all the points in one series.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class ChartPointCollection implements Iterable
```
Represents a collection that contains all the points in one series.
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
ChartPointCollection points = chart.getNSeries().get(0).getPoints();
for (int i = 0; i <points.getCount(); i++)
{
//Get Data Point
ChartPoint point = points.get(i);
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
| [clear()](#clear--) | Remove all setting of the chart points. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [ChartPoint](../../com.aspose.cells/chartpoint) element at the specified index in the series. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the chart point. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Returns an enumerator for the entire [ChartPointCollection](../../com.aspose.cells/chartpointcollection). |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes point at the index of the series.. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```
Remove all setting of the chart points.
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
### get(int index) {#get-int-}
```
public ChartPoint get(int index)
```
Gets the [ChartPoint](../../com.aspose.cells/chartpoint) element at the specified index in the series.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of chart point in the series. |
**Returns:**
[ChartPoint](../../com.aspose.cells/chartpoint) - The ChartPoint object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the count of the chart point.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```
Returns an enumerator for the entire [ChartPointCollection](../../com.aspose.cells/chartpointcollection).
**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes point at the index of the series..
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the point. |
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
