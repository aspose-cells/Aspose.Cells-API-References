##VerticalPageBreakCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VerticalPageBreakCollection extends CollectionBase
```
Encapsulates a collection of [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int column)](#add-int-) | Adds a vertical page break to the collection. |
| [add(int row, int column)](#add-int-int-) | Adds a vertical page break to the collection. |
| [add(int startRow, int endRow, int column)](#add-int-int-int-) | Adds a vertical page break to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String cellName)](#add-java.lang.String-) | Adds a vertical page break to the collection. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) element at the specified index. |
| [get(String cellName)](#get-java.lang.String-) | Gets the [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) element with the specified cell name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the VPageBreak element at a specified name. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int column) {#add-int-}
```
public int add(int column)
```
Adds a vertical page break to the collection.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Cell column index, zero based. |
**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) object index.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```
Adds a vertical page break to the collection.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index, zero based. |
| column | int | Cell column index, zero based. |
**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) object index.
### add(int startRow, int endRow, int column) {#add-int-int-int-}
```
public int add(int startRow, int endRow, int column)
```
Adds a vertical page break to the collection.
**Remarks**
This method is used to add a vertical pagebreak within a print area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index, zero based. |
| endRow | int | End row index, zero based. |
| column | int | Column index, zero based. |
**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) object index.
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```
Adds a vertical page break to the collection.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) object index.
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
### get(int index) {#get-int-}
```
public VerticalPageBreak get(int index)
```
Gets the [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public VerticalPageBreak get(String cellName)
```
Gets the [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) element with the specified cell name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element with the specified cell name.
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
Removes the VPageBreak element at a specified name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Element index, zero based. |
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
