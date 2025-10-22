##HyperlinkCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```
Encapsulates a collection of [Hyperlink](../../com.aspose.cells/hyperlink) objects.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(0);
//Get Hyperlinks Collection
HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
//Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Adds a hyperlink to a specified cell or a range of cells. |
| [clear()](#clear--) | Clears all hyperlinks. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Hyperlink](../../com.aspose.cells/hyperlink) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove the hyperlink at the specified index in this collection. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```
Adds a hyperlink to a specified cell or a range of cells.
**Example**
```
//Instantiating a Workbook object
Workbook excel = new Workbook();
Worksheet worksheet = excel.getWorksheets().get(0);
worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int | First row of the hyperlink range. |
| firstColumn | int | First column of the hyperlink range. |
| totalRows | int | Number of rows in this hyperlink range. |
| totalColumns | int | Number of columns of this hyperlink range. |
| address | java.lang.String | Address of the hyperlink. |
**Returns:**
int - [Hyperlink](../../com.aspose.cells/hyperlink) object index.
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
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
| totalRows | int | Number of rows in this hyperlink range. |
| totalColumns | int | Number of columns of this hyperlink range. |
| address | java.lang.String | Address of the hyperlink. |
**Returns:**
int - [Hyperlink](../../com.aspose.cells/hyperlink) object index.
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```
Adds a hyperlink to a specified cell or a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | The top-left cell of the range. |
| endCellName | java.lang.String | The bottom-right cell of the range. |
| address | java.lang.String | Address of the hyperlink. |
| textToDisplay | java.lang.String | The text to be displayed for the specified hyperlink. |
| screenTip | java.lang.String | The screenTip text for the specified hyperlink. |
**Returns:**
int - [Hyperlink](../../com.aspose.cells/hyperlink) object index.
### clear() {#clear--}
```
public void clear()
```
Clears all hyperlinks.
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
public Hyperlink get(int index)
```
Gets the [Hyperlink](../../com.aspose.cells/hyperlink) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove the hyperlink at the specified index in this collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
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
