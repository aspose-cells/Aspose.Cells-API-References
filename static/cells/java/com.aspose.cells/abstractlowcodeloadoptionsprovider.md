##AbstractLowCodeLoadOptionsProvider
Implementation to provide multiple load options for processes that use multiple inputssuch as template files.
**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```
Implementation to provide multiple load options for processes that use multiple inputs(such as template files).
**Remarks**
For example, [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) feature requires multiple template files to merge.
## Constructors
| Constructor | Description |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Releases resources after processing currently part of input. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Gets the load options from which to load data of currently processed part. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Checks whether there is more input. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
```
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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```
Releases resources after processing currently part of input.
**Remarks**
By default this method just closes the stream specified by the [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) directly(if the load options specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | the load options used for currently split part. |
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```
Gets the load options from which to load data of currently processed part.
**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```
Checks whether there is more input.
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
