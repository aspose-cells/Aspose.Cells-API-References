##CellValueFormatStrategy
Specifies how to apply style for the value of the cell.
**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```
Specifies how to apply style for the value of the cell.
## Fields
| Field | Description |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Only formatted with the cell's original style. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Gets the displayed string shown in ms excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Formatted with the cell's displayed style. |
| [NONE](#NONE) | Not formatted. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```
Only formatted with the cell's original style.
### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```
Gets the displayed string shown in ms excel. The main difference from [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "\#" may be shown, just like what ms excel does.
### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```
Formatted with the cell's displayed style.
### NONE {#NONE}
```
public static final int NONE
```
Not formatted.
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
