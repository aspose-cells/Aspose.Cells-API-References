##TextOverflowType
Represents the way the text vertical or horizontal overflow.
**Inheritance:**
java.lang.Object
```
public final class TextOverflowType
```
Represents the way the text vertical or horizontal overflow.
## Fields
| Field | Description |
| --- | --- |
| [CLIP](#CLIP) | Pay attention to top and bottom barriers. |
| [ELLIPSIS](#ELLIPSIS) | Pay attention to top and bottom barriers. |
| [OVERFLOW](#OVERFLOW) | Overflow the text and pay no attention to top and bottom barriers. |
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
### CLIP {#CLIP}
```
public static final int CLIP
```
Pay attention to top and bottom barriers. Provide no indication that there is text which is not visible.
### ELLIPSIS {#ELLIPSIS}
```
public static final int ELLIPSIS
```
Pay attention to top and bottom barriers. Use an ellipsis to denote that there is text which is not visible. Only for vertical overflow.
### OVERFLOW {#OVERFLOW}
```
public static final int OVERFLOW
```
Overflow the text and pay no attention to top and bottom barriers.
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
