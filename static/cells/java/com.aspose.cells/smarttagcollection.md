##SmartTagCollection
Represents all smart tags in the cell.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SmartTagCollection extends CollectionBase
```
Represents all smart tags in the cell.
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String uri, String name)](#add-java.lang.String-java.lang.String-) | Adds a smart tag. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets a [SmartTag](../../com.aspose.cells/smarttag) object at the specific index |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column of the cell smart tags. |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getRow()](#getRow--) | Gets the row of the cell smart tags. |
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
### add(String uri, String name) {#add-java.lang.String-java.lang.String-}
```
public int add(String uri, String name)
```
Adds a smart tag.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | java.lang.String | Specifies the namespace URI of the smart tag |
| name | java.lang.String | Specifies the name of the smart tag. |
**Returns:**
int - The index of smart tag in the list.
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
public SmartTag get(int index)
```
Gets a [SmartTag](../../com.aspose.cells/smarttag) object at the specific index
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
**Returns:**
[SmartTag](../../com.aspose.cells/smarttag) - returns a [SmartTag](../../com.aspose.cells/smarttag) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```
Gets the column of the cell smart tags.
**Returns:**
int
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of elements contained in the CollectionBase instance.
**Returns:**
int - The number of elements contained in the CollectionBase instance.
### getRow() {#getRow--}
```
public int getRow()
```
Gets the row of the cell smart tags.
**Returns:**
int
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
