---
title: FileFormatUtil
second_title: Aspose.Cells for Java API Reference
description: Provides utility methods for converting file format enums to strings or file extensions and back.
type: docs
url: /java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Provides utility methods for converting file format enums to strings or file extensions and back.
## Methods

| Method | Description |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Detects and returns the information about a format of an excel stored in a stream. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Detects and returns the information about a format of an excel stored in a stream. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Detects and returns the information about a format of an excel stored in a file. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Detects and returns the information about a format of an excel stored in a file. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Converts a file name extension into a SaveFormat value. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Converting file format to save format. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Converts a load format enumerated value into a file extension. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Converts a LoadFormat value to a SaveFormat value if possible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Converts a save format enumerated value into a file extension. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Converts a SaveFormat value to a LoadFormat value if possible. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Detects and returns the information about a format of an excel stored in a stream. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Detects and returns the information about a format of an excel stored in a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Detects and returns the information about a format of an excel stored in a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | The password for encrypted ooxml files. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Detects and returns the information about a format of an excel stored in a file.

**Remarks**

Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Detects and returns the information about a format of an excel stored in a file.

**Remarks**

Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| password | java.lang.String | The password for encrypted ooxml files. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Converts a file name extension into a SaveFormat value.

**Remarks**

If the extension cannot be recognized, returns [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | java.lang.String | The file extension. Can be with or without a leading dot. Case-insensitive. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Converting file format to save format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). The file format type. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
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
### isTemplateFormat(String extension) {#isTemplateFormat-java.lang.String-}
```
public static boolean isTemplateFormat(String extension)
```


Returns true if the extension is .xlt, .xltX, .xltm,.ots.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean - 
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Converts a load format enumerated value into a file extension.

**Remarks**

If it can not be converted, returns null.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). The loaded file format. |

**Returns:**
java.lang.String - The returned extension is a lower-case string with a leading dot.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Converts a LoadFormat value to a SaveFormat value if possible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). The load format. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). The save format.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveFormatToExtension(int format) {#saveFormatToExtension-int-}
```
public static String saveFormatToExtension(int format)
```


Converts a save format enumerated value into a file extension.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). The save format. |

**Returns:**
java.lang.String - The returned extension is a lower-case string with a leading dot.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Converts a SaveFormat value to a LoadFormat value if possible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). The save format. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). The load format
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(InputStream stream, String password) {#verifyPassword-java.io.InputStream-java.lang.String-}
```
public static boolean verifyPassword(InputStream stream, String password)
```


Detects and returns the information about a format of an excel stored in a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | The password for encrypted ooxml files. |

**Returns:**
boolean - Returns whether the password is corrected.
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

