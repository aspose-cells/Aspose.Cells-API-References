##LowCodeHtmlSaveOptions
Options for saving html in low code way.
**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```
Options for saving html in low code way.
## Constructors
| Constructor | Description |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | The general options for saving html. |
| [getOutputFile()](#getOutputFile--) | Gets the file(with path if needed) for saving the generated data. |
| [getOutputStream()](#getOutputStream--) | Gets the Stream for writing the generated data to. |
| [getSaveFormat()](#getSaveFormat--) | Gets the format of spreadsheet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | The general options for saving html. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Sets the file(with path if needed) for saving the generated data. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Sets the Stream for writing the generated data to. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Sets the format of spreadsheet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```
The general options for saving html.
**Remarks**
When one [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) instance is specified, the [SaveFormat](../../com.aspose.cells/saveformat) will be overwritten(if it had been specified before).
**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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
Gets the format of spreadsheet.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
When changing this property, the save format specified by [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) will be ignored(if it had been specified before).
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
### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```
The general options for saving html.
**Remarks**
When one [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) instance is specified, the [SaveFormat](../../com.aspose.cells/saveformat) will be overwritten(if it had been specified before).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |
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
Sets the format of spreadsheet.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
When changing this property, the save format specified by [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) will be ignored(if it had been specified before).
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
