##RowColumnEventArgs
Provides data for row/column events.
**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```
Provides data for row/column events.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | The argument of the event. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | The row or column number, starts from zero. |
| [getType()](#getType--) | The row or column type. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | shall we cancel the operation. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Call this method in RowDeleting/ColumnDeleting event handlers to cancel the deleting operations. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```
The argument of the event.
**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```
The row or column number, starts from zero.
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
The row or column type.
See [RowColumnType](../../com.aspose.gridweb/rowcolumntype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```
shall we cancel the operation.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```
Call this method in RowDeleting/ColumnDeleting event handlers to cancel the deleting operations.
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
