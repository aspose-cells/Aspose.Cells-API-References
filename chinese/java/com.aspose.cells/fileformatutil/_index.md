---
title: "FileFormatUtil"
second_title: "Aspose.Cells for Java API 参考"
description: "提供将文件格式枚举转换为字符串或文件扩展名以及反向转换的实用方法。"
type: docs
url: /zh/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

提供将文件格式枚举转换为字符串或文件扩展名以及反向转换的实用方法。
## 方法

| 方法 | 描述 |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | 检测并返回存储在流中的 Excel 格式信息。 |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | 检测并返回存储在流中的 Excel 格式信息。 |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | 检测并返回存储在文件中的 Excel 格式信息。 |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | 检测并返回存储在文件中的 Excel 格式信息。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | 将文件扩展名转换为 SaveFormat 值。 |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | 将文件格式转换为保存格式。 |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | 如果扩展名是 .xlt、.xltX、.xltm、.ots，则返回 true。 |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | 将加载格式枚举值转换为文件扩展名。 |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | 如果可能，将 LoadFormat 值转换为 SaveFormat 值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | 将保存格式枚举值转换为文件扩展名。 |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | 如果可能，将 SaveFormat 值转换为 LoadFormat 值。 |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | 检测并返回存储在流中的 Excel 格式信息。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


检测并返回存储在流中的 Excel 格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 流 |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


检测并返回存储在流中的 Excel 格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| 密码 | java.lang.String | 加密 ooxml 文件的密码。 |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


检测并返回存储在文件中的 Excel 格式信息。

**Remarks**

仅支持检查带有魔术签名的部分文件。如果没有魔术签名，则无法精确检测文件格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


检测并返回存储在文件中的 Excel 格式信息。

**Remarks**

仅支持检查带有魔术签名的部分文件。如果没有魔术签名，则无法精确检测文件格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径。 |
| 密码 | java.lang.String | 加密 ooxml 文件的密码。 |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


将文件扩展名转换为 SaveFormat 值。

**Remarks**

如果无法识别扩展名，则返回 [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extension | java.lang.String | 文件扩展名。可以带或不带前导点。大小写不敏感。 |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat)。
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


将文件格式转换为保存格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). 文件格式类型。 |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat)。
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


如果扩展名是 .xlt、.xltX、.xltm、.ots，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


将加载格式枚举值转换为文件扩展名。

**Remarks**

如果无法转换，返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). 已加载的文件格式。 |

**Returns:**
java.lang.String - 返回的扩展名是带前导点的小写字符串。
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


如果可能，将 LoadFormat 值转换为 SaveFormat 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). 加载格式。 |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). 保存格式。
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


将保存格式枚举值转换为文件扩展名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). 保存格式。 |

**Returns:**
java.lang.String - 返回的扩展名是带前导点的小写字符串。
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


如果可能，将 SaveFormat 值转换为 LoadFormat 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). 保存格式。 |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). 加载格式
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


检测并返回存储在流中的 Excel 格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| 密码 | java.lang.String | 加密 ooxml 文件的密码。 |

**Returns:**
boolean - 返回密码是否已更正。
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

