##SetBorderPosition
Represents the border position to be set of a cells range.
**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```
Represents the border position to be set of a cells range.
**Example**
```
GridWeb GridWeb1=new GridWeb();
GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Fields
| Field | Description |
| --- | --- |
| [BOTTOM](#BOTTOM) | Bottom border |
| [CROSS](#CROSS) | Cross borders |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Bottom border |
| [LEFT](#LEFT) | Left border |
| [NONE](#NONE) | No borders |
| [OUTLINE](#OUTLINE) | VerticalMiddle borders |
| [RIGHT](#RIGHT) | Right border |
| [TOP](#TOP) | Top border |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | HorizontalMiddle borders |
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
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```
Bottom border
### CROSS {#CROSS}
```
public static final int CROSS
```
Cross borders
### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```
Bottom border
### LEFT {#LEFT}
```
public static final int LEFT
```
Left border
### NONE {#NONE}
```
public static final int NONE
```
No borders
### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```
VerticalMiddle borders
### RIGHT {#RIGHT}
```
public static final int RIGHT
```
Right border
### TOP {#TOP}
```
public static final int TOP
```
Top border
### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```
HorizontalMiddle borders
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
