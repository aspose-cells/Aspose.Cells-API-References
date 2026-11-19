---
title: "IGridJsService"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在控制器操作中使用的基本操作 API 接口。"
type: docs
url: /zh/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

表示在控制器操作中使用的基本操作 API 接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | 应用从本地文件添加图像的操作。 |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | 执行从远程 URL 添加图像的操作。 |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | 检查工作簿实例是否在内存缓存中。此方法仅适用于协作模式。 |
| [clearAllJsonCache()](#clearAllJsonCache--) | 清除所有 JSON 缓存条目（内存和磁盘）。 |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | 清除属于指定唯一 ID 的所有 JSON 缓存条目。 |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | 应用复制图像的操作。 |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | 获取指定唯一 ID 的文件的 JSON 字符串。 |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | 将工作簿的 JSON 字符串写入流 |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | 根据指定的唯一 ID 将文件的 JSON 字符串写入流。 |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | 应用下载文件的操作 |
| [getFile(String fileid)](#getFile-java.lang.String-) | 获取文件流 |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | 获取图像流。 |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | 获取图像 URL。 |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件中指定工作表的 JSON 字符串。 |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 将缓存中文件中指定工作表的 JSON 字符串写入流。 |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | 使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。 |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | 获取嵌入式 OLE 对象的字节数组数据。 |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | 应用更新操作。 |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
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
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


执行从远程 URL 添加图像的操作。

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
public abstract boolean checkInCacheForCollaborative(String uid)
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
public abstract void clearAllJsonCache()
```


清除所有 JSON 缓存条目（内存和磁盘）。

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


清除所有属于指定唯一 ID 的 JSON 缓存条目。在带外修改源文件后调用此方法，以便下一个请求重新生成 JSON。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


应用复制图像的操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | JSON 字符串参数 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String - JSON 字符串结果
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


获取指定唯一 ID 的文件的 JSON 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 文件路径 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


将工作簿的 JSON 字符串写入流

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| filePath | java.lang.String | 文件路径 |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


根据指定的唯一 ID 将文件的 JSON 字符串写入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 将被写入的流 |
| filePath | java.lang.String | 文件路径 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


获取文件流

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileid | java.lang.String | 文件 ID |

**Returns:**
java.io.InputStream - 文件的流
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
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
public abstract String imageUrl(String baseURL, String picid, String uid)
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
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public abstract String load(String uid, String filename)
```


使用指定的唯一 ID 从缓存中获取文件的 JSON 字符串，并在 JSON 中设置输出文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| filename | java.lang.String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |

**Returns:**
java.lang.String - JSON 字符串
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
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
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


应用更新操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | java.lang.String | 更新操作的 JSON 格式字符串。 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String
