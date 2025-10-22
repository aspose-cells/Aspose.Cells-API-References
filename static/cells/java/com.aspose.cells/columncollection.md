##ColumnCollection
Collection of the  objects that represent the individual columnsettings in a worksheet.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ColumnCollection extends CollectionBase
```
Collection of the [Column](../../com.aspose.cells/column) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
//Add new Style to Workbook
Style style = workbook.createStyle();
//Setting the background color to Blue
style.setForegroundColor(Color.getBlue());
//setting Background Pattern
style.setPattern(BackgroundType.SOLID);
//New Style Flag
StyleFlag styleFlag = new StyleFlag();
//Set All Styles
styleFlag.setAll(true);
//Change the default width of first ten columns
for (int i = 0; i ? i++)
{
worksheet.getCells().getColumns().get(i).setWidth(20);
}
//Get the Column with non default formatting
ColumnCollection columns = worksheet.getCells().getColumns();
for (Column column : (Iterable<Column>) columns)
{
//Apply Style to first ten Columns
column.applyStyle(style, styleFlag);
}
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int columnIndex)](#get-int-) | Gets a [Column](../../com.aspose.cells/column) object by column index. |
| [getByIndex(int index)](#getByIndex-int-) | Gets the column object by the index. |
| [getClass()](#getClass--) |  |
| [getColumnByIndex(int index)](#getColumnByIndex-int-) | Gets the [Column](../../com.aspose.cells/column) object by the position in the list. |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
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
### clear() {#clear--}
```
public void clear()
```
Removes all objects from the CollectionBase instance.
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
### get(int columnIndex) {#get-int-}
```
public Column get(int columnIndex)
```
Gets a [Column](../../com.aspose.cells/column) object by column index. The Column object of given column index will be instantiated if it does not exist before.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int |  |
**Returns:**
[Column](../../com.aspose.cells/column)
### getByIndex(int index) {#getByIndex-int-}
```
public Column getByIndex(int index)
```
Gets the column object by the index.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex() method. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumnByIndex(int index) {#getColumnByIndex-int-}
```
public Column getColumnByIndex(int index)
```
Gets the [Column](../../com.aspose.cells/column) object by the position in the list.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position in the list. |
**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
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
Removes the item at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |
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
