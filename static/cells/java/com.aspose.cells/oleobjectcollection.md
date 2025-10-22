##OleObjectCollection
Represents embedded OLE objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class OleObjectCollection extends CollectionBase
```
Represents embedded OLE objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData)](#add-int-int-int-int-byte---) | Adds an OleObject to the collection. |
| [add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData, String linkedFile)](#add-int-int-int-int-byte---java.lang.String-) | Adds a linked OleObject to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Remove all embedded OLE objects. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [OleObject](../../com.aspose.cells/oleobject) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the element at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData) {#add-int-int-int-int-byte---}
```
public int add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData)
```
Adds an OleObject to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| height | int | Height of oleObject, in unit of pixel. |
| width | int | Width of oleObject, in unit of pixel. |
| imageData | byte[] | Image of ole object as byte array. |
**Returns:**
int - [OleObject](../../com.aspose.cells/oleobject) object index.
### add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData, String linkedFile) {#add-int-int-int-int-byte---java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int height, int width, byte[] imageData, String linkedFile)
```
Adds a linked OleObject to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| height | int | Height of oleObject, in unit of pixel. |
| width | int | Width of oleObject, in unit of pixel. |
| imageData | byte[] | Image of ole object as byte array. |
| linkedFile | java.lang.String |  |
**Returns:**
int - [OleObject](../../com.aspose.cells/oleobject) object index.
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
Remove all embedded OLE objects.
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
public OleObject get(int index)
```
Gets the [OleObject](../../com.aspose.cells/oleobject) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - The element at the specified index.
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
Removes the element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The specified index. |
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
