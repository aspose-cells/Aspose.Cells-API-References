##CellValueType
Specifies a cell value type.
**Inheritance:**
java.lang.Object
```
public final class CellValueType
```
Specifies a cell value type.
## Fields
| Field | Description |
| --- | --- |
| [IS_BOOL](#IS-BOOL) | Cell value is boolean. |
| [IS_DATE_TIME](#IS-DATE-TIME) | Cell value is datetime. |
| [IS_ERROR](#IS-ERROR) | Cell contains error value. |
| [IS_NULL](#IS-NULL) | Blank cell. |
| [IS_NUMERIC](#IS-NUMERIC) | Cell value is numeric. |
| [IS_STRING](#IS-STRING) | Cell value is string. |
| [IS_UNKNOWN](#IS-UNKNOWN) | Cell value type is unknown. |
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
### IS_BOOL {#IS-BOOL}
```
public static final int IS_BOOL
```
Cell value is boolean. Corresponding value must be bool.
### IS_DATE_TIME {#IS-DATE-TIME}
```
public static final int IS_DATE_TIME
```
Cell value is datetime. Corresponding value must be DateTime.
### IS_ERROR {#IS-ERROR}
```
public static final int IS_ERROR
```
Cell contains error value. Corresponding value must be error string.
### IS_NULL {#IS-NULL}
```
public static final int IS_NULL
```
Blank cell. Corresponding value should be null.
### IS_NUMERIC {#IS-NUMERIC}
```
public static final int IS_NUMERIC
```
Cell value is numeric. Corresponding value must be int or double.
### IS_STRING {#IS-STRING}
```
public static final int IS_STRING
```
Cell value is string. Corresponding value must be string.
### IS_UNKNOWN {#IS-UNKNOWN}
```
public static final int IS_UNKNOWN
```
Cell value type is unknown.
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
