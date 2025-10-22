##TxtLoadStyleStrategy
Specifies how to apply style for parsed values when converting string value to number or datetime.
**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```
Specifies how to apply style for parsed values when converting string value to number or datetime.
## Fields
| Field | Description |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Set the style as built-in number/datetime when the parsed value are plain numeric/datetime values. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Set the exact custom format for the parsed value to make the formatted value be same with the original input one. |
| [NONE](#NONE) | Does not set style for the parsed value. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```
Set the style as built-in number/datetime when the parsed value are plain numeric/datetime values.
**Remarks**
When ms excel parsing datetime or numeric values according to user's input(such as CSV file), the formatting of those values may be changed, such as leading/tailing zeros of number, year/month/day order of datetime, ...etc. This type is for simulating ms excel's behavior.
### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```
Set the exact custom format for the parsed value to make the formatted value be same with the original input one.
### NONE {#NONE}
```
public static final int NONE
```
Does not set style for the parsed value.
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
