##NameCollection
Represents a collection of all the  objects in the spreadsheet.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```
Represents a collection of all the [Name](../../com.aspose.cells/name) objects in the spreadsheet.
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String text)](#add-java.lang.String-) | Defines a new name. |
| [clear()](#clear--) | Remove all defined names which are not referenced by the formulas and data source. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Gets all defined name by scope. |
| [get(int index)](#get-int-) | Gets the [Name](../../com.aspose.cells/name) element at the specified index. |
| [get(String text)](#get-java.lang.String-) | Gets the [Name](../../com.aspose.cells/name) element with the specified name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Remove the name. |
| [remove(String[] names)](#remove-java.lang.String---) | Remove an array of name |
| [removeAt(int index)](#removeAt-int-) | Remove the name at the specific index. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Remove the duplicate defined names |
| [sort()](#sort--) | Sorts defined names. |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```
Defines a new name.
**Remarks**
Name cannot include spaces and cannot look like cell references.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text to use as the name. |
**Returns:**
int - [Name](../../com.aspose.cells/name) object index.
### clear() {#clear--}
```
public void clear()
```
Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them.
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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```
Gets all defined name by scope.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). The scope type. |
| sheetIndex | int | The sheet index. Only effects when scope type is [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) |
**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```
Gets the [Name](../../com.aspose.cells/name) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```
Gets the [Name](../../com.aspose.cells/name) element with the specified name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | Name text. |
**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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
### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```
Remove the name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The name text. |
### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```
Remove an array of name
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| names | java.lang.String[] | The names' text. |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove the name at the specific index.
**Remarks**
Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | index of the Name to be removed. |
### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```
Remove the duplicate defined names
### sort() {#sort--}
```
public void sort()
```
Sorts defined names.
**Remarks**
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
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
