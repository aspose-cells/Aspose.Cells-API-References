##TxtValueQuoteType
Specifies the type of using quotation marks for values in text format files.
**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```
Specifies the type of using quotation marks for values in text format files.
## Fields
| Field | Description |
| --- | --- |
| [ALWAYS](#ALWAYS) | All values will be quoted always. |
| [MINIMUM](#MINIMUM) | Only quote values when needed. |
| [NEVER](#NEVER) | All values will not be quoted. |
| [NORMAL](#NORMAL) | All values that contain special characters such as quotation mark, separator character will be quoted. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```
All values will be quoted always.
### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```
Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted.
### NEVER {#NEVER}
```
public static final int NEVER
```
All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent.
### NORMAL {#NORMAL}
```
public static final int NORMAL
```
All values that contain special characters such as quotation mark, separator character will be quoted. Same with the behavior of ms excel for exporting text file.
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
