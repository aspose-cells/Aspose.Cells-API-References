##GridPictureCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridPictureCollection
```
Encapsulates a collection of [GridPicture](../../com.aspose.gridweb/gridpicture) objects.
## Methods
| Method | Description |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Adds a picture to the collection. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName)](#add-int-int-java.lang.String-) | Adds a picture to the collection. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Adds a picture to the collection. |
| [clear()](#clear--) | Clear all pictures. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridPicture](../../com.aspose.gridweb/gridpicture) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets the rows enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int param_int)](#removeAt-int-) | Remove shapes at the specific index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)
```
Adds a picture to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |
| fileName | java.lang.String | Image filename. |
**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) object index.
### add(int upperLeftRow, int upperLeftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName)
```
Adds a picture to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| fileName | java.lang.String | Image filename. |
**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) object index.
### add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)
```
Adds a picture to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| fileName | java.lang.String | Image filename. |
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |
**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) object index.
### clear() {#clear--}
```
public void clear()
```
Clear all pictures.
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
public GridPicture get(int index)
```
Gets the [GridPicture](../../com.aspose.gridweb/gridpicture) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridPicture](../../com.aspose.gridweb/gridpicture) - The element at the specified index.
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
### removeAt(int param_int) {#removeAt-int-}
```
public void removeAt(int param_int)
```
Remove shapes at the specific index
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_int | int |  |
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
