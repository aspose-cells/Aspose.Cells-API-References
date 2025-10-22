##ShapePathType
Represents path segment type.
**Inheritance:**
java.lang.Object
```
public final class ShapePathType
```
Represents path segment type.
## Fields
| Field | Description |
| --- | --- |
| [ARC_TO](#ARC-TO) | An arc |
| [CLOSE](#CLOSE) | If the starting POINT and the end POINT are not the same, a single straight line is drawn to connect the starting POINT and ending POINT of the path. |
| [CUBIC_BEZIER_CURVE_TO](#CUBIC-BEZIER-CURVE-TO) | Cubic Bezier curve |
| [END](#END) | The end of the current path |
| [ESCAPE](#ESCAPE) | Escape |
| [LINE_TO](#LINE-TO) | Straight line segment |
| [MOVE_TO](#MOVE-TO) | Start a new path |
| [UNKNOWN](#UNKNOWN) | Unknown |
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
### ARC_TO {#ARC-TO}
```
public static final int ARC_TO
```
An arc
### CLOSE {#CLOSE}
```
public static final int CLOSE
```
If the starting POINT and the end POINT are not the same, a single straight line is drawn to connect the starting POINT and ending POINT of the path.
### CUBIC_BEZIER_CURVE_TO {#CUBIC-BEZIER-CURVE-TO}
```
public static final int CUBIC_BEZIER_CURVE_TO
```
Cubic Bezier curve
### END {#END}
```
public static final int END
```
The end of the current path
### ESCAPE {#ESCAPE}
```
public static final int ESCAPE
```
Escape
### LINE_TO {#LINE-TO}
```
public static final int LINE_TO
```
Straight line segment
### MOVE_TO {#MOVE-TO}
```
public static final int MOVE_TO
```
Start a new path
### UNKNOWN {#UNKNOWN}
```
public static final int UNKNOWN
```
Unknown
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
