##LowCodeImageSaveOptions
Options for saving image in low code way.
**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```
Options for saving image in low code way.
## Constructors
| Constructor | Description |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | The options for rendering images. |
| [getOutputFile()](#getOutputFile--) | Gets the file(with path if needed) for saving the generated data. |
| [getOutputStream()](#getOutputStream--) | Gets the Stream for writing the generated data to. |
| [getSaveFormat()](#getSaveFormat--) | Gets the save format. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Provider of save options for saving generated images. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | The options for rendering images. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Sets the file(with path if needed) for saving the generated data. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Sets the Stream for writing the generated data to. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Sets the save format. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Provider of save options for saving generated images. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```
The options for rendering images.
**Remarks**
When one [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) instance is specified, the [SaveFormat](../../com.aspose.cells/saveformat) will be overwritten(if it had been specified before).
**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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
Gets the save format.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
If [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) has been specified, setting this property will also change the [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) value of it.
**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```
Provider of save options for saving generated images.
**Remarks**
The output([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) or [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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
### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```
The options for rendering images.
**Remarks**
When one [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) instance is specified, the [SaveFormat](../../com.aspose.cells/saveformat) will be overwritten(if it had been specified before).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |
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
Sets the save format.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
If [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) has been specified, setting this property will also change the [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) value of it.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```
Provider of save options for saving generated images.
**Remarks**
The output([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) or [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |
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
