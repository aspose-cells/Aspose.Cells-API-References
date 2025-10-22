##StreamProviderOptions
Represents the stream options.
**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```
Represents the stream options.
## Constructors
| Constructor | Description |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Initializes a new instance of the [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) class. |
| [StreamProviderOptions()](#StreamProviderOptions--) | Initializes a new instance of the [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) class. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | The user custom path(URL) saved in generated html file for the referred source. |
| [getDefaultPath()](#getDefaultPath--) | The default path(URL) saved in generated html file for the referred source. |
| [getInputStream()](#getInputStream--) | Gets the input stream to get data. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Gets the type of loading resource. |
| [getStream()](#getStream--) | Gets the output stream to write saved data. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | The user custom path(URL) saved in generated html file for the referred source. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Sets the input stream to get data. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Sets the type of loading resource. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Sets the output stream to write saved data. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```
Initializes a new instance of the [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) class.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). The type to load the linked resource. |
| defaultPath | java.lang.String | The default path. |
### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```
Initializes a new instance of the [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) class.
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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```
The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.
**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```
The default path(URL) saved in generated html file for the referred source. For example, the sheet data saved in xxx\_files/sheet001.htm, the url used in the main html file should be like "src="xxx\_files/sheet001.htm""
**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```
Gets the input stream to get data.
**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```
Gets the type of loading resource.
See [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).
**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```
Gets the output stream to write saved data.
**Returns:**
java.io.OutputStream
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
### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```
The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```
Sets the input stream to get data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.io.InputStream |  |
### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```
Sets the type of loading resource.
See [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```
Sets the output stream to write saved data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.io.OutputStream |  |
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
