##DataSorterKey
Represents the key of the data sorter.
**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```
Represents the key of the data sorter.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets the sorted color. |
| [getIconId()](#getIconId--) | Represents the id of the icon set type. |
| [getIconSetType()](#getIconSetType--) | Represents the icon set type. |
| [getIndex()](#getIndex--) | Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder()](#getOrder--) | Indicates the order of sorting. |
| [getType()](#getType--) | Represents the type of sorting. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```
Gets the sorted color.
**Remarks**
Only takes effect when [CellValue.getType()](../../com.aspose.cells/cellvalue\#getType--) is [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) or [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).
**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```
Represents the id of the icon set type.
**Remarks**
Only takes effect when [CellValue.getType()](../../com.aspose.cells/cellvalue\#getType--) is [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).
**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```
Represents the icon set type.
See [IconSetType](../../com.aspose.cells/iconsettype).
**Remarks**
Only takes effect when [CellValue.getType()](../../com.aspose.cells/cellvalue\#getType--) is [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).
**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```
Gets the sorted column index(absolute position, column A is 0, B is 1, ...).
**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```
Indicates the order of sorting.
See [SortOrder](../../com.aspose.cells/sortorder).
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
Represents the type of sorting.
See [SortOnType](../../com.aspose.cells/sortontype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
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
