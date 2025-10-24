##DataSorter
Summary description for DataSorter.
**Inheritance:**
java.lang.Object
```
public class DataSorter
```
Summary description for DataSorter.
**Example**
```
//Instantiate a new Workbook object.
Workbook workbook = new Workbook("Book1.xls");
//Get the workbook datasorter object.
DataSorter sorter = workbook.getDataSorter();
//Set the first order for datasorter object.
sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
//Define the first key.
sorter.setKey1(0);
//Set the second order for datasorter object.
sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
//Define the second key.
sorter.setKey2(1);
//Create a cells area (range).
CellArea ca = new CellArea();
//Specify the start row index.
ca.StartRow = 0;
//Specify the start column index.
ca.StartColumn = 0;
//Specify the last row index.
ca.EndRow = 13;
//Specify the last column index.
ca.EndColumn = 1;
//Sort data in the specified data range (A1:B14)
sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
//Save the excel file.
workbook.save("outBook.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Adds color sort key. |
| [addKey(int key, int order)](#addKey-int-int-) | Adds sorted column index and sort order. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Adds sorted column index and sort order with custom sort list. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Adds sorted column index and sort order with custom sort list. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Adds sorted column index and sort order with custom sort list. |
| [clear()](#clear--) | Clear all settings. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Gets whether case sensitive when comparing string. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKey2()](#getKey2--) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKey3()](#getKey3--) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKeys()](#getKeys--) | Gets the key list of data sorter. |
| [getOrder1()](#getOrder1--) | Represents sort order of the first key. |
| [getOrder2()](#getOrder2--) | Represents sort order of the second key. |
| [getOrder3()](#getOrder3--) | Represents sort order of the third key. |
| [getSortAsNumber()](#getSortAsNumber--) | Indicates whether sorting anything that looks like a number. |
| [getSortLeftToRight()](#getSortLeftToRight--) | True means that sorting orientation is from left to right. |
| [hasHeaders()](#hasHeaders--) | Represents whether the range has headers. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Sets whether case sensitive when comparing string. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Represents whether the range has headers. |
| [setKey1(int value)](#setKey1-int-) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Represents sort order of the first key. |
| [setOrder2(int value)](#setOrder2-int-) | Represents sort order of the second key. |
| [setOrder3(int value)](#setOrder3-int-) | Represents sort order of the third key. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Indicates whether sorting anything that looks like a number. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | True means that sorting orientation is from left to right. |
| [sort()](#sort--) | Sort the data in the range. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Sort the data of the area. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Sorts the data of the area. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```
Adds color sort key.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). The sorted color value type. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). The sort order. |
| color | [Color](../../com.aspose.cells/color) | The custom sort color. |
### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```
Adds sorted column index and sort order.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). The sort order |
### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```
Adds sorted column index and sort order with custom sort list.
**Remarks**
If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). The sorted value type. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). The sort order. |
| customList | java.lang.Object | The custom sort list. |
### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```
Adds sorted column index and sort order with custom sort list.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). The sort order. |
| customList | java.lang.String | The custom sort list. |
### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```
Adds sorted column index and sort order with custom sort list.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). The sort order. |
| customList | java.lang.String[] | The custom sort list. |
### clear() {#clear--}
```
public void clear()
```
Clear all settings.
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```
Gets whether case sensitive when comparing string.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```
Represents first sorted column index(absolute position, column A is 0, B is 1, ...).
**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```
Represents second sorted column index(absolute position, column A is 0, B is 1, ...).
**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```
Represents third sorted column index(absolute position, column A is 0, B is 1, ...).
**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```
Gets the key list of data sorter.
**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```
Represents sort order of the first key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```
Represents sort order of the second key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```
Represents sort order of the third key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```
Indicates whether sorting anything that looks like a number.
**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```
True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.
**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```
Represents whether the range has headers.
**Returns:**
boolean
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
### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```
Sets whether case sensitive when comparing string.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```
Represents whether the range has headers.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```
Represents first sorted column index(absolute position, column A is 0, B is 1, ...).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```
Represents second sorted column index(absolute position, column A is 0, B is 1, ...).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```
Represents third sorted column index(absolute position, column A is 0, B is 1, ...).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```
Represents sort order of the first key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```
Represents sort order of the second key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```
Represents sort order of the third key.
See [SortOrder](../../com.aspose.cells/sortorder).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```
Indicates whether sorting anything that looks like a number.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```
True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### sort() {#sort--}
```
public int[] sort()
```
Sort the data in the range.
**Returns:**
int[] - the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```
Sort the data of the area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | The cells contains the data area. |
| area | [CellArea](../../com.aspose.cells/cellarea) | The area needed to sort |
**Returns:**
int[] - the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```
Sorts the data of the area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | The cells contains the data area. |
| startRow | int | The start row of the area. |
| startColumn | int | The start column of the area. |
| endRow | int | The end row of the area. |
| endColumn | int | The end column of the area. |
**Returns:**
int[] - the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
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
