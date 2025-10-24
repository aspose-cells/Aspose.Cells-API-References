##MergedCellsShrinkType
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
**Inheritance:**
java.lang.Object
```
public final class MergedCellsShrinkType
```
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
## Fields
| Field | Description |
| --- | --- |
| [KEEP_HEADER_ONLY](#KEEP-HEADER-ONLY) | Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |
| [NONE](#NONE) | Leaves the merged cells as it is without any modification. |
| [SHRINK_TO_FIT](#SHRINK-TO-FIT) | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible. |
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
### KEEP_HEADER_ONLY {#KEEP-HEADER-ONLY}
```
public static final int KEEP_HEADER_ONLY
```
Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank.
### NONE {#NONE}
```
public static final int NONE
```
Leaves the merged cells as it is without any modification.
### SHRINK_TO_FIT {#SHRINK-TO-FIT}
```
public static final int SHRINK_TO_FIT
```
Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible.
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
