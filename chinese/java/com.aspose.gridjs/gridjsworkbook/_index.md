---
title: "GridJsWorkbook"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 GridJs 的主要入口类"
type: docs
url: /zh/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

表示 GridJs 的主要入口类
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | 创建 GridJsWorkbook 的新实例。 |
## 字段

| 字段 | 描述 |
| --- | --- |
| [CacheImp](#CacheImp) | 用于缓存存储的自定义实现，如果您想以流方式存储缓存，需要进行设置和实现。 |
| [CalculateEngine](#CalculateEngine) | 计算引擎的自定义实现，如果您想进行自定义计算，需要进行设置并实现它。 |
| [PICTURE_TYPE](#PICTURE-TYPE) | 图像类型的 const 值 |
| [UpdateMonitor](#UpdateMonitor) | 获取/设置用于跟踪更新操作的更新监视器 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | 通过删除编辑形状及其目标形状或清除目标单元格范围内容，执行（应用）工作簿中的所有编辑操作。 |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | 检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。 |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | 复制图像或形状。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | 获取 JSON 格式的错误消息字符串。 |
| [exportToJson()](#exportToJson--) | 从内存数据获取 JSON 字符串，JSON 中的默认文件名为：book1。 |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | 从内存数据获取 JSON 字符串，设置 JSON 中的输出文件名。 |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | 从内存数据获取 JSON 字符串，设置 JSON 中的输出文件名。 |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | 获取用于存储电子表格文件的缓存目录。 |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | 通过文件扩展名获取加载格式 |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | 获取图像流。 |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | 获取图像 URL。 |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。 |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | 获取嵌入式 OLE 对象的字节数组数据。 |
| [getSettings()](#getSettings--) | 表示工作簿设置。 |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | 使用给定的文件名为文件缓存生成新的唯一 ID。 |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | 使用加载格式从文件流导入 Excel 文件。 |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | 使用加载格式和打开密码从文件流导入 Excel 文件。 |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | 从文件路径导入 excel 文件。 |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | 从文件流导入 excel 文件。 |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | 使用加载格式和打开密码从文件流导入 Excel 文件。 |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | 从文件路径导入 excel 文件。 |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | 从文件路径导入 excel 文件并使用打开密码。 |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | 从 JSON 格式字符串导入 excel 文件。 |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | 从文件流或 URL 在工作表中插入图像（必须提供文件流或 URL），或在 p.type 为 AutoShapeType 之一时插入形状。 |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | 从内存中的 Workbook 生成 JSON 并写入指定的流。 |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中检索文件的 JSON 字符串，在 JSON 中设置输出文件名，并将其写入流。 |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件中指定工作表的 JSON 字符串。 |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中检索文件中指定工作表的 JSON 字符串，并将其写入流。 |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | 对内存数据应用批量更新。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | 根据 JSON 操作数组对 Excel 文件执行编辑操作。 |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | 将内存数据保存到具有指定文件名的缓存文件，并设置打开密码，保存格式基于文件名的扩展名。 |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | 将内存数据保存到流，保存格式基于原始文件格式。 |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | 将内存数据保存到文件路径，如果文件有扩展名，保存格式基于该扩展名。 |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | 将内存数据保存到流，保存格式为 html。 |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | 将内存数据保存到文件路径，保存格式为 html。 |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | 将内存数据保存到流，保存格式为 pdf。 |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | 将内存数据保存到文件路径，保存格式为 pdf。 |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | 将内存数据保存到流，保存格式为 xlsx。 |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | 将内存数据保存到文件路径，保存格式为 xlsx。 |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | 设置用于存储电子表格文件的缓存目录。 |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | 设置从控制器获取基础图像的操作 URL。 |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | 为加载操作设置 InterruptMonitor。 |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | 为保存操作设置 InterruptMonitor。 |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | 表示工作簿设置。 |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | 设置工作簿中编辑形状的透明度。 |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | 将工作表中所有字符串值翻译为目标语言 |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | 应用更新操作。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


创建 GridJsWorkbook 的新实例。

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


用于缓存存储的自定义实现，如果您想以流方式存储缓存，需要进行设置和实现。

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


计算引擎的自定义实现，如果您想进行自定义计算，需要进行设置并实现它。

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


图像类型的 const 值

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


获取/设置用于跟踪更新操作的更新监视器

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


通过删除编辑形状及其目标形状或清除目标单元格范围内容，执行（应用）工作簿中的所有编辑操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| excelFilePath | java.lang.String | Excel 文件的文件路径。 |
| uid | java.lang.String | 工作簿的唯一标识符。如果为 null 或为空，将基于文件路径生成新的 uid。 |

### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


复制图像或形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| p | java.lang.String | 用于指定单元格位置的操作的 JSON 字符串，它包含工作表名称、图像或形状的左上行、左上列\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - 新复制图像的 JSON 字符串
### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


获取 JSON 格式的错误消息字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| msg | java.lang.String | 错误信息。 |

**Returns:**
java.lang.String - JSON 字符串。
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


从内存数据获取 JSON 字符串，JSON 中的默认文件名为：book1。

**Returns:**
java.lang.String - JSON 字符串。
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


从内存数据获取 JSON 字符串，设置 JSON 中的输出文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filename | java.lang.String | 指定 JSON 中的文件名。如果设置为 null，默认文件名为：book1.. |

**Returns:**
java.lang.String - JSON 字符串。
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


从内存数据获取 JSON 字符串，设置 JSON 中的输出文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filename | java.lang.String | 指定 JSON 中的文件名。如果设置为 null，默认文件名为：book1.. |

**Returns:**
java.lang.StringBuilder - JSON StringBuilder。
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filename | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


获取用于存储电子表格文件的缓存目录。如果未设置，则使用来自 [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) 或 [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) 的静态属性。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


通过文件扩展名获取加载格式

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extension | java.lang.String | 文件扩展名，通常以 '.' 开头。 |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat)。
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


获取图像流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| picid | java.lang.String | 图像 ID。 |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - 图像流
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


获取图像 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| picid | java.lang.String | 图像 ID。 |
| delimiter | java.lang.String | 字符串分隔符。 |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |

**Returns:**
java.lang.StringBuilder - JSON 字符串 StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
```


获取嵌入式 OLE 对象的字节数组数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| sheetname | java.lang.String | 工作表名称。 |
| oleid | int | 嵌入式 ole 对象的 ID。 |
| label | java.lang.String | 嵌入式 ole 对象的显示标签。 |

**Returns:**
byte[] - 嵌入式 ole 对象的字节数组数据。
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


表示工作簿设置。

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


使用给定的文件名为文件缓存生成新的唯一 ID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件名。 |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


使用加载格式从文件流导入 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件流 | java.io.InputStream | Excel 文件的流。 |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat)。Excel 文件的 LoadFormat。 |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


使用加载格式和打开密码从文件流导入 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件流 | java.io.InputStream | Excel 文件的流。 |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat)。Excel 文件的 LoadFormat。 |
| 密码 | java.lang.String | Excel 文件的打开密码。如果未设置密码，值可以为 null。 |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


从文件路径导入 excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件的完整路径。 |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


从文件流导入 excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一标识，如果设置为 null，将自动生成。 |
| 文件流 | java.io.InputStream | Excel 文件的流。 |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat)。Excel 文件的 LoadFormat。 |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


使用加载格式和打开密码从文件流导入 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一标识，如果设置为 null，将自动生成。 |
| 文件流 | java.io.InputStream | Excel 文件的流。 |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat)。Excel 文件的 LoadFormat。 |
| 密码 | java.lang.String | Excel 文件的打开密码。如果未设置密码，值可以为 null。 |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


从文件路径导入 excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一标识，如果设置为 null，将自动生成。 |
| fileName | java.lang.String | 文件的完整路径。 |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


从文件路径导入 excel 文件并使用打开密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一标识，如果设置为 null，将自动生成。 |
| fileName | java.lang.String | 文件的完整路径。 |
| 密码 | java.lang.String | Excel 文件的打开密码。如果未设置密码，值可以为 null。 |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


从 JSON 格式字符串导入 excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| json | java.lang.String | JSON 格式字符串。 |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


从文件流或 URL 在工作表中插入图像（必须提供文件流或 URL），或在 p.type 为 AutoShapeType 之一时插入形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一标识 |
| p | java.lang.String | 用于指定图像单元格位置、工作表名称、左上行、左上列的操作的 JSON 格式字符串\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | 图像文件的文件流 |
| imageUrl | java.lang.String | 图像文件的 URL |

**Returns:**
java.lang.String - 插入图像的 JSON 格式字符串
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


从内存中的 Workbook 生成 JSON 并写入指定的流。可选地缓存生成的 JSON，以加快后续检索。与 JsonToStreamByUid 的关键区别：- 此方法使用当前内存中的 Workbook 状态（wb 字段）- JsonToStreamByUid 从磁盘上的 .cells 缓存文件重新加载 Workbook- 当您希望在修改后导出当前工作簿状态时使用此方法- 当需要从先前缓存的文件状态重新生成 JSON 时使用 JsonToStreamByUid 缓存行为（提供 uid 时）：- 在生成前检查 JSON 缓存（L1 内存 + L2 磁盘）- 如果缓存未命中，则从内存中的工作簿生成 JSON- 将生成的 JSON 存入缓存以供后续请求使用

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 用于写入 JSON 数据的输出流 |
| filename | java.lang.String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| filename | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


使用指定的唯一 ID 从缓存中检索文件的 JSON 字符串，在 JSON 中设置输出文件名，并将其写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


使用指定的唯一 ID 从缓存中获取文件中指定工作表的 JSON 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| sheetName | java.lang.String | 工作表名称。 |

**Returns:**
java.lang.StringBuilder - JSON 字符串 StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


使用指定的唯一 ID 从缓存中检索文件中指定工作表的 JSON 字符串，并将其写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| sheetName | java.lang.String | 工作表名称。 |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


对内存数据应用批量更新。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| json | java.lang.String | 更新的 JSON 格式字符串。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


根据 JSON 操作数组对 Excel 文件执行编辑操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| excelFilePath | java.lang.String | 待编辑的 Excel 文件的文件路径。 |
| uid | java.lang.String | 工作簿的唯一标识符。如果为 null 或为空，将基于文件路径生成新的 uid。 |
| arrayOfRedactionOpr | java.lang.String[] | 表示要应用的编辑操作的 JSON 字符串数组。 |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


将内存数据保存到具有指定文件名的缓存文件，并设置打开密码，保存格式基于文件名的扩展名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 要保存的文件名。 |
| 密码 | java.lang.String | Excel 文件的打开密码。若未设置密码，值可以为 null。 |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


将内存数据保存到流，保存格式基于原始文件格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 用于保存的流。 |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


将内存数据保存到文件路径，如果文件有扩展名，保存格式基于该扩展名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 用于保存的文件路径。 |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


将内存数据保存到流，保存格式为 html。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 用于保存的流。 |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


将内存数据保存到文件路径，保存格式为 html。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 用于保存的文件路径。 |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


将内存数据保存到流，保存格式为 pdf。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 用于保存的流。 |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


将内存数据保存到文件路径，保存格式为 pdf。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 用于保存的文件路径。 |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


将内存数据保存到流，保存格式为 xlsx。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 用于保存的流。 |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


将内存数据保存到文件路径，保存格式为 xlsx。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | 用于保存的文件路径。 |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


设置用于存储电子表格文件的缓存目录。如果未设置，则使用来自 [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) 或 [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) 的静态属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


设置从控制器获取基础图像的操作 URL。

**Remarks**

当 CacheImp 为 null 时，需要设置此项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseImageURL | java.lang.String | 获取基础图像的操作 URL。 |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


为加载操作设置 InterruptMonitor。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor 实例。 |
| calculateTimeoutMilliseconds | int | 加载文件的超时时间（毫秒）。 |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


为保存操作设置 InterruptMonitor。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor 实例。 |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


表示工作簿设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


设置工作簿中编辑形状的透明度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| excelFilePath | java.lang.String | Excel 文件的文件路径。 |
| uid | java.lang.String | 工作簿的唯一标识符。如果为 null 或为空，将基于文件路径生成新的 uid。 |
| isTransparent | boolean | 如果为 true，则将透明度设置为 0.89（半透明）；如果为 false，则将透明度设置为 1（完全不透明/不可见）。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


将工作表中所有字符串值翻译为目标语言

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| sheetName | java.lang.String | 工作表名称 |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | 实现 translate 功能的翻译器 |
| targetLanguage | java.lang.String | 目标语言 |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


应用更新操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | 更新操作的 JSON 格式字符串。 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String - 更新结果的 JSON 格式字符串。
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

