##SeriesCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```
Encapsulates a collection of [Series](../../com.aspose.cells/series) objects.
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
chart.getNSeries().add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.getNSeries().setCategoryData("C1:C4");
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String area, boolean isVertical)](#add-java.lang.String-boolean-) | Adds the [Series](../../com.aspose.cells/series) collection to a chart. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Adds the [Series](../../com.aspose.cells/series) collection to a chart. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Adds the [Series](../../com.aspose.cells/series) collection to a chart. |
| [changeColors(int type)](#changeColors-int-) | Set Monochromatic Palette for chart series. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Directly changes the orders of the two series. |
| [clear()](#clear--) | Clears the collection |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Series](../../com.aspose.cells/series) element at the specified index. |
| [getCategoryData()](#getCategoryData--) | Gets the range of category Axis values. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Gets the range of second category Axis values. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Gets the [Series](../../com.aspose.cells/series) element by order. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [isColorVaried()](#isColorVaried--) | Represents if the color of points is varied. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove at a series at the specific index. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Sets the range of category Axis values. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Represents if the color of points is varied. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Sets the range of second category Axis values. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Sets the name of all the serieses in the chart. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Directly changes the orders of the two series. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String area, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String area, boolean isVertical)
```
Adds the [Series](../../com.aspose.cells/series) collection to a chart.
**Remarks**
If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.
If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
**Returns:**
int - Return the first index of the added ASeries in the NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```
Adds the [Series](../../com.aspose.cells/series) collection to a chart.
**Remarks**
If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.
If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |
**Returns:**
int - Return the first index of the added ASeries in the NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```
Adds the [Series](../../com.aspose.cells/series) collection to a chart.
**Remarks**
If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].
If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | java.lang.String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
**Returns:**
int - Return the first index of the added ASeries in the NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```
Set Monochromatic Palette for chart series.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). The Monochromatic Type. |
### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```
Directly changes the orders of the two series.
**Remarks**
NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |
### clear() {#clear--}
```
public void clear()
```
Clears the collection
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
public Series get(int index)
```
Gets the [Series](../../com.aspose.cells/series) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```
Gets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"\{2,6,8,10\}").
**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```
Gets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"\{2,6,8,10\}"). Only effects when some ASerieses plot on the second axis.
**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```
Gets the [Series](../../com.aspose.cells/series) element by order.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| order | int | The order of series |
**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```
Represents if the color of points is varied.
**Returns:**
boolean
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
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove at a series at the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```
Sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"\{2,6,8,10\}").
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```
Represents if the color of points is varied.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```
Sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"\{2,6,8,10\}"). Only effects when some ASerieses plot on the second axis.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```
Sets the name of all the serieses in the chart.
**Remarks**
If the start index is larger than the count of the serieses, it will return and do nothing.
If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.
If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the first series which you want to set the name. |
| area | java.lang.String | Specifies the area for the series name. |
| isVertical | boolean | >Specifies whether to plot the series from a range of cell values by row or by column. |
### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```
Directly changes the orders of the two series.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |
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
