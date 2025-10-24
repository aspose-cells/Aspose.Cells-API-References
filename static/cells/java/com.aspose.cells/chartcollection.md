##ChartCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```
Encapsulates a collection of [Chart](../../com.aspose.cells/chart) objects.
**Example**
```
Workbook workbook = new Workbook();
ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Methods
| Method | Description |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Adds a chart with preset template. |
| [add(int type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#add-int-int-int-int-int-) | Adds a chart to the collection. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Adds a chart to the collection. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Adds a chart to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Adds a chart to the collection. |
| [clear()](#clear--) | Clear all charts. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Chart](../../com.aspose.cells/chart) element at the specified index. |
| [get(String name)](#get-java.lang.String-) | Gets the chart by the name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Remove the specific chart. |
| [removeAt(int index)](#removeAt-int-) | Remove a chart at the specific index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```
Adds a chart with preset template.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The data of chart template file(.crtx). |
| dataRange | java.lang.String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |
**Returns:**
int - [Chart](../../com.aspose.cells/chart) object index.
### add(int type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```
Adds a chart to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Chart type |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |
**Returns:**
int - [Chart](../../com.aspose.cells/chart) object index.
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```
Adds a chart to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Chart type |
| dataRange | java.lang.String | Specifies the data range of the chart |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |
**Returns:**
int - [Chart](../../com.aspose.cells/chart) object index.
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```
Adds a chart to the collection.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-) property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Chart type |
| dataRange | java.lang.String | Specifies the data range of the chart |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| rightRow | int | Lower right row index |
| bottomColumn | int | Lower right column index |
**Returns:**
int - [Chart](../../com.aspose.cells/chart) object index.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```
Adds an item to the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |
**Returns:**
int - The position into which the new element was inserted.
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```
Adds a chart to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Chart type |
| left | int | The x offset to corner |
| top | int | The y offset to corner |
| width | int | The chart width |
| height | int | The chart height |
**Returns:**
int - [Chart](../../com.aspose.cells/chart) object index.
### clear() {#clear--}
```
public void clear()
```
Clear all charts.
### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```
Return whether instance contains this object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |
**Returns:**
boolean - Whether instance contains this object
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
public Chart get(int index)
```
Gets the [Chart](../../com.aspose.cells/chart) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```
Gets the chart by the name.
**Remarks**
The default chart name is null. So you have to explicitly set the name of the chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The chart name. |
**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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
Gets the number of elements contained in the CollectionBase instance.
**Returns:**
int - The number of elements contained in the CollectionBase instance.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```
Determines the index of a specific item in the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |
**Returns:**
int - The index of value if found in the list; otherwise, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```
Returns an enumerator that iterates through the CollectionBase instance.
**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```
Remove the specific chart.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove a chart at the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The chart index. |
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
