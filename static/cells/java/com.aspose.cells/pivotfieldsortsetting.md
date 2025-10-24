##PivotFieldSortSetting
Represents the setting of sorting pivot fields.
**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```
Represents the setting of sorting pivot fields.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Sorts by the values in which row or column. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Represents the index of the field sorted by |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | The pivot line type sorted by. |
| [getSortType()](#getSortType--) | Represents the [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Indicates whether a simple data sort operation will be applied. |
| [isSortByLabels()](#isSortByLabels--) | Indicates whether sorting the field by itself or data field. |
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
### getCell() {#getCell--}
```
public String getCell()
```
Sorts by the values in which row or column.
**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```
Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.
**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```
The pivot line type sorted by.
See [PivotLineType](../../com.aspose.cells/pivotlinetype).
**Remarks**
Only works when not sorting this field by labels.
**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```
Represents the [SortOrder](../../com.aspose.cells/sortorder).
See [SortOrder](../../com.aspose.cells/sortorder).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```
Indicates whether a simple data sort operation will be applied.
**Remarks**
The default value is true.
**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```
Indicates whether sorting the field by itself or data field.
**Returns:**
boolean
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
