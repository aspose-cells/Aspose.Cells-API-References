##RowCollection
Collects the  objects that represent the individual rows in a worksheet.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```
Collects the [Row](../../com.aspose.cells/row) objects that represent the individual rows in a worksheet.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
//Get first row
Row row = worksheet.getCells().getRows().get(0);
```
## Methods
| Method | Description |
| --- | --- |
| [clear()](#clear--) | Clear all rows and cells. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Gets a [Row](../../com.aspose.cells/row) object by given row index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of rows in this collection. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Gets the row object by the position in the list. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets an enumerator that iterates rows through this collection |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Gets an enumerator that iterates rows through this collection |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove the row item at the specified index(position) in this collection. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```
Clear all rows and cells.
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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```
Gets a [Row](../../com.aspose.cells/row) object by given row index. The Row object of given row index will be instantiated if it does not exist before.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int |  |
**Returns:**
[Row](../../com.aspose.cells/row)
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
Gets the number of rows in this collection.
**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```
Gets the row object by the position in the list.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position. |
**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
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
Gets an enumerator that iterates rows through this collection
**Example**
```
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.getWorksheets().get(0).getCells();
Iterator en = cells.getRows().iterator();
while (en.hasNext())
{
Row row = (Row)en.next();
System.out.println(row.getIndex() + ": " + row.getHeight());
}
```
**Returns:**
java.util.Iterator - The row enumerator which will traverse all existing rows in this collection.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```
Gets an enumerator that iterates rows through this collection
**Remarks**
If the row collection will be modified(by operations that may cause new Row be instantiated or existing Row be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | boolean | whether enumerate rows in reversed order |
| sync | boolean | whether the returned enumerator should check the modification of row collection and keep synchronized with it. |
**Returns:**
java.util.Iterator - The row enumerator which will traverse all existing rows in this collection.
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
Remove the row item at the specified index(position) in this collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | zero-based index(position, not [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) of the existing row item in this collection. |
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
