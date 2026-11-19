---
title: "GridJsService"
second_title: "Aspose.Cells for Java API 参考"
description: "提供在控制器操作中使用的基本操作 API。"
type: docs
url: /zh/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

提供在控制器操作中使用的基本操作 API。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | GridJsService 的默认构造函数 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | 应用从本地文件添加图像的操作。 |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | 应用从本地文件添加图像的操作。 |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | 检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。 |
| [clearAllJsonCache()](#clearAllJsonCache--) | 清除所有 JSON 缓存条目（内存和磁盘）。 |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | 清除属于指定唯一 ID 的所有 JSON 缓存条目。 |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | 应用复制图像的操作。 |
| [destroy()](#destroy--) | 此方法仅适用于 Java，它实现了 DisposableBean 中的 destroy 方法，该方法将在 Spring 完成请求后自动调用，实际上它会调用 Dispose 方法。 |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | 获取指定唯一 ID 的文件的 JSON 字符串。 |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | 将文件的 JSON 字符串写入流。 |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | 根据指定的唯一 ID 将文件的 JSON 字符串写入流。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | 应用下载文件的操作 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | 获取文件流 |
| [getSettings()](#getSettings--) | 表示工作簿设置。 |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | 获取图像流。 |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | 获取图像 URL。 |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件中指定工作表的 JSON 字符串。 |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 将缓存中文件中指定工作表的 JSON 字符串写入流。 |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | 获取嵌入式 OLE 对象的字节数组数据。 |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | 表示工作簿设置。 |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | 将工作表中所有字符串值翻译为目标语言 |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | 应用更新操作。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


GridJsService 的默认构造函数

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
```


应用从本地文件添加图像的操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | JSON 字符串参数 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| 文件流 | java.io.InputStream | 图像的文件流 |

**Returns:**
java.lang.String - JSON 字符串结果
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


应用从本地文件添加图像的操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | JSON 字符串参数 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| 文件流 | java.io.InputStream | 图像的文件流 |
| imageurl | java.lang.String | 指定图像 URL。 |

**Returns:**
java.lang.String - JSON 字符串结果
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


清除所有 JSON 缓存条目（内存和磁盘）。

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


清除所有属于指定唯一 ID 的 JSON 缓存条目。在带外修改源文件后调用此方法，以便下一个请求重新生成 JSON。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


应用复制图像的操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | JSON 字符串参数 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String - JSON 字符串结果
### destroy() {#destroy--}
```
public void destroy()
```


此方法仅适用于 Java，它实现了 DisposableBean 中的 destroy 方法，该方法将在 Spring 完成请求后自动调用，实际上它会调用 Dispose 方法。

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


获取指定唯一 ID 的文件的 JSON 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 完整文件路径 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


将文件的 JSON 字符串写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| filePath | java.lang.String | 完整文件路径 |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


根据指定的唯一 ID 将文件的 JSON 字符串写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| filePath | java.lang.String | 完整文件路径 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
```


应用下载文件的操作

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | JSON 参数 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 文件名 |

**Returns:**
java.lang.String - 文件 URL
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


获取文件流

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileid | java.lang.String | 文件 ID |

**Returns:**
java.io.InputStream - 文件的流
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


表示工作簿设置。

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
```


获取图像流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| picid | java.lang.String | 图像 ID。 |

**Returns:**
java.io.InputStream - 图像流
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public String imageUrl(String baseURL, String picid, String uid)
```


获取图像 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseURL | java.lang.String | 基础操作 URL。 |
| picid | java.lang.String | 图像 ID。 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String - 图像 URL
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String sheetName, String uid)
```


使用指定的唯一 ID 从缓存中获取文件中指定工作表的 JSON 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表名称。 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


使用指定的唯一 ID 将缓存中文件中指定工作表的 JSON 字符串写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| sheetName | java.lang.String | 工作表名称。 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public String load(String uid, String filename)
```


使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |

**Returns:**
java.lang.String - JSON 字符串
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
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
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


表示工作簿设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

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

