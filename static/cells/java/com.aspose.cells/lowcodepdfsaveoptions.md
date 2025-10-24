##LowCodePdfSaveOptions
Options for saving pdf in low code way.
**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```
Options for saving pdf in low code way.
## Constructors
| Constructor | Description |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Gets the file(with path if needed) for saving the generated data. |
| [getOutputStream()](#getOutputStream--) | Gets the Stream for writing the generated data to. |
| [getPdfOptions()](#getPdfOptions--) | The options for saving Pdf file. |
| [getSaveFormat()](#getSaveFormat--) | The save format for the output. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Sets the file(with path if needed) for saving the generated data. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Sets the Stream for writing the generated data to. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | The options for saving Pdf file. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | The save format for the output. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```
The options for saving Pdf file.
**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```
The save format for the output. For converting to pdf, it can only be [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).
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
### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```
The options for saving Pdf file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |
### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```
The save format for the output. For converting to pdf, it can only be [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).
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
