##HtmlCrossType
Represents five types of html cross string.
**Inheritance:**
java.lang.Object
```
public final class HtmlCrossType
```
Represents five types of html cross string.
## Fields
| Field | Description |
| --- | --- |
| [CROSS](#CROSS) | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| [CROSS_HIDE_RIGHT](#CROSS-HIDE-RIGHT) | Display HTML cross string and hide the right string when the texts overlap. |
| [DEFAULT](#DEFAULT) | Display like MS Excel,depends on the next cell. |
| [FIT_TO_CELL](#FIT-TO-CELL) | Only displaying the string within the width of cell. |
| [MS_EXPORT](#MS-EXPORT) | Display the string like MS Excel exporting html. |
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
### CROSS {#CROSS}
```
public static final int CROSS
```
Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell.
### CROSS_HIDE_RIGHT {#CROSS-HIDE-RIGHT}
```
public static final int CROSS_HIDE_RIGHT
```
Display HTML cross string and hide the right string when the texts overlap.
### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```
Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated
### FIT_TO_CELL {#FIT-TO-CELL}
```
public static final int FIT_TO_CELL
```
Only displaying the string within the width of cell.
### MS_EXPORT {#MS-EXPORT}
```
public static final int MS_EXPORT
```
Display the string like MS Excel exporting html.
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
