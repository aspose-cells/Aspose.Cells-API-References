##GridNameCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```
Encapsulates a collection of [GridName](../../com.aspose.gridweb/gridname) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Defines a new name in the specified sheet. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Defines a new global name. |
| [clear()](#clear--) | Removes all Names; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridName](../../com.aspose.gridweb/gridname) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets the rows enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Remove an array of name |
| [removeAt(int index)](#removeAt-int-) | Remove the name at the specific index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```
Defines a new name in the specified sheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The sheet index that the name is applyed in. |
| text | java.lang.String | Name text.It can not have sheetname . |
| refersTo | java.lang.String | The formula that the name is defined to refer to.It must have sheetname .eg.'sheet hello!'A1:B2. |
**Returns:**
int - Name object index.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```
Defines a new global name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | Name text.It can have sheetname . |
| refersTo | java.lang.String | The formula that the name is defined to refer to.It must have a sheetname .eg.'sheet hello!'A1:B2. |
**Returns:**
int - Name object index.
### clear() {#clear--}
```
public void clear()
```
Removes all Names;
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
public GridName get(int index)
```
Gets the [GridName](../../com.aspose.gridweb/gridname) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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
Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred,please only set Name.RefersTo as null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
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
