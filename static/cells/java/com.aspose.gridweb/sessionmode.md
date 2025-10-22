##SessionMode
Represents the session mode of the grid.
**Inheritance:**
java.lang.Object
```
public final class SessionMode
```
Represents the session mode of the grid.
## Fields
| Field | Description |
| --- | --- |
| [CUSTOM](#CUSTOM) | Uses the LoadCustomData event to load the grid's sheet data manually. |
| [FILE](#FILE) | Uses the system file to store/recover the grid's sheet data automatically,user need to set SessionStorePath to specify the file directory. |
| [SESSION](#SESSION) | Uses the system session to store/recover the grid's sheet data automatically. |
| [VIEW_STATE](#VIEW-STATE) | Uses the page's viewstate to store/recover the grid's sheet data automatically. |
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
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```
Uses the LoadCustomData event to load the grid's sheet data manually. And uses the SheetDataUpdated event to save the grid's sheet data.
### FILE {#FILE}
```
public static final int FILE
```
Uses the system file to store/recover the grid's sheet data automatically,user need to set SessionStorePath to specify the file directory.
### SESSION {#SESSION}
```
public static final int SESSION
```
Uses the system session to store/recover the grid's sheet data automatically.
### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```
Uses the page's viewstate to store/recover the grid's sheet data automatically.
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
