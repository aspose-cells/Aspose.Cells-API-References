##DataBarAxisPosition
Specifies the axis position for a range of cells with conditional formatting as data bars.
**Inheritance:**
java.lang.Object
```
public final class DataBarAxisPosition
```
Specifies the axis position for a range of cells with conditional formatting as data bars.
## Fields
| Field | Description |
| --- | --- |
| [AUTOMATIC](#AUTOMATIC) | Display the axis at a variable position based on the ratio of the minimum negative value to the maximum positive value in the range. |
| [MIDPOINT](#MIDPOINT) | Display the axis at the midpoint of the cell regardless of the set of values in the range. |
| [NONE](#NONE) | No axis is displayed, and both positive and negative values are displayed in the left-to-right direction. |
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
### AUTOMATIC {#AUTOMATIC}
```
public static final int AUTOMATIC
```
Display the axis at a variable position based on the ratio of the minimum negative value to the maximum positive value in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction. When all values are positive or all values are negative, no axis is displayed.
### MIDPOINT {#MIDPOINT}
```
public static final int MIDPOINT
```
Display the axis at the midpoint of the cell regardless of the set of values in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction.
### NONE {#NONE}
```
public static final int NONE
```
No axis is displayed, and both positive and negative values are displayed in the left-to-right direction.
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
