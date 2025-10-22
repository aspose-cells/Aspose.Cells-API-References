##GridCommentCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridCommentCollection
```
Encapsulates a collection of [GridComment](../../com.aspose.gridweb/gridcomment) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Adds a comment to the collection. |
| [add(String cellName)](#add-java.lang.String-) | Adds a comment to the collection. |
| [clear()](#clear--) | Removes all comments; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified index. |
| [get(int row, int column)](#get-int-int-) | Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified row index and column index. |
| [get(String cellName)](#get-java.lang.String-) | Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified cell. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets the rows enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int row, int column)](#removeAt-int-int-) | Removes the comment of the specific cell. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Removes the comment of the specific cell. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```
Adds a comment to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Cell row index. |
| column | int | Cell column index. |
**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) object index.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```
Adds a comment to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) object index.
### clear() {#clear--}
```
public void clear()
```
Removes all comments;
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
public GridComment get(int index)
```
Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public GridComment get(int row, int column)
```
Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified row index and column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public GridComment get(String cellName)
```
Gets the [GridComment](../../com.aspose.gridweb/gridcomment) element at the specified cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Cell name. |
**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
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
Gets the size of enumerator
**Returns:**
int
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
Gets the rows enumerator
**Returns:**
java.util.Iterator - The rows enumerator
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```
Removes the comment of the specific cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | the column index. |
### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```
Removes the comment of the specific cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | The name of cell which contains a comment. |
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
