##LowCodeSaveOptions
Options for saving generated results in low code way.
**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```
Options for saving generated results in low code way.
## Constructors
| Constructor | Description |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Gets the file(with path if needed) for saving the generated data. |
| [getOutputStream()](#getOutputStream--) | Gets the Stream for writing the generated data to. |
| [getSaveFormat()](#getSaveFormat--) | Gets the save format for the output. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Sets the file(with path if needed) for saving the generated data. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Sets the Stream for writing the generated data to. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Sets the save format for the output. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```
Gets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) will be ignored.
**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```
Gets the Stream for writing the generated data to. When setting this property with value other than null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) will be ignored.
**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```
Gets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Returns:**
int
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
### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```
Sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) will be ignored.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```
Sets the Stream for writing the generated data to. When setting this property with value other than null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) will be ignored.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.io.InputStream |  |
### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```
Sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
