##ReConnectionMethodType
Specifies what the spreadsheet application should do when a connection fails.
**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```
Specifies what the spreadsheet application should do when a connection fails.
## Fields
| Field | Description |
| --- | --- |
| [ALWAYS](#ALWAYS) | On every refresh get updated connection information from the external connection file, if available, and use that instead of the existing connection information. |
| [NEVER](#NEVER) | Never get updated connection information from the external connection file even if it is available and even if the existing connection information is invalid |
| [REQUIRED](#REQUIRED) | On refresh use the existing connection information and if it ends up being invalid then get updated connection information, if available from the external connection file. |
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
On every refresh get updated connection information from the external connection file, if available, and use that instead of the existing connection information. In this case the data refresh will fail if the external connection file is unavailable.
### NEVER {#NEVER}
```
public static final int NEVER
```
Never get updated connection information from the external connection file even if it is available and even if the existing connection information is invalid
### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```
On refresh use the existing connection information and if it ends up being invalid then get updated connection information, if available from the external connection file.
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
