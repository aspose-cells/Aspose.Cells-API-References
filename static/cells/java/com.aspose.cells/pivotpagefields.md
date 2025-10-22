##PivotPageFields
Represents the pivot page field items  if the pivot table data source is consolidation ranges.
**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```
Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.
## Constructors
| Constructor | Description |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Represents the pivot page field items. |
## Methods
| Method | Description |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Sets which item label in each page field to use to identify the data range. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Adds a page field. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Gets the number of page fields. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```
Represents the pivot page field items.
### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```
Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | int | The consolidation data range index. |
| pageItemIndex | int[] | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |
### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```
Adds a page field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageItems | java.lang.String[] | Page field item label |
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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```
Gets the number of page fields.
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
