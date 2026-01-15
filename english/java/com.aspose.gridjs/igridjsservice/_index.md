---
title: IGridJsService
second_title: Aspose.Cells for Java API Reference
description: Reprensents the basic operation apis interface used in controller actions.
type: docs
url: /java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Reprensents the basic operation apis interface used in controller actions.
## Methods

| Method | Description |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Applies the add image from local file operation. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Applies the add image from remote URL operation. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Applies the copy image operation. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Gets JSON string for the file by the specified unique id. . |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Write the JSON string for the Workbook to the stream |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Write the JSON string for the file to the stream by the specified unique id. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Applies the download file operation |
| [getFile(String fileid)](#getFile-java.lang.String-) | Get file stream |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Get Stream of image. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Gets the image URL. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Gets the JSON string of the specified sheet in the file from the cache using the specified unique id. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Writes the JSON string of the specified sheet in the file from the cache using the specified unique id to the stream.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Gets the byte array data of the embedded ole object . |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applies the update operation. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
```


Applies the add image from local file operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON string parameter |
| uid | java.lang.String | The unique id for the file cache. |
| filestream | java.io.InputStream | The filestream of the image |

**Returns:**
java.lang.String - The JSON string result
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Applies the add image from remote URL operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON string parameter |
| uid | java.lang.String | The unique id for the file cache. |
| filestream | java.io.InputStream | The filestream of the image |
| imageurl | java.lang.String | Specify the image URL. |

**Returns:**
java.lang.String - The JSON string result
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public abstract boolean checkInCacheForCollaborative(String uid)
```


Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean - 
### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Applies the copy image operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON string parameter |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.String - The JSON string result
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Gets JSON string for the file by the specified unique id. .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Write the JSON string for the Workbook to the stream

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| filePath | java.lang.String | The file path |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Write the JSON string for the file to the stream by the specified unique id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| filePath | java.lang.String | The file path |
| uid | java.lang.String | The unique id for the file cache. |

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
```


Applies the download file operation

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON parameter |
| uid | java.lang.String | The unique id for the file cache. |
| filename | java.lang.String | The file name |

**Returns:**
java.lang.String - The file URL
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Get file stream

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileid | java.lang.String | the file id |

**Returns:**
java.io.InputStream - The stream of the file
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
```


Get Stream of image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| picid | java.lang.String | The image id. |

**Returns:**
java.io.InputStream - The image stream
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String imageUrl(String baseURL, String picid, String uid)
```


Gets the image URL.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseURL | java.lang.String | The base action URL. |
| picid | java.lang.String | The image id. |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.String - The image URL
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Gets the JSON string of the specified sheet in the file from the cache using the specified unique id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | the sheet name. |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Writes the JSON string of the specified sheet in the file from the cache using the specified unique id to the stream..

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| sheetName | java.lang.String | The sheet name. |
| uid | java.lang.String | The unique id for the file cache. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public abstract String load(String uid, String filename)
```


Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |

**Returns:**
java.lang.String - The JSON string
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
```


Gets the byte array data of the embedded ole object .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| sheetname | java.lang.String | The worksheet name. |
| oleid | int | The id for the embedded ole object. |
| label | java.lang.String | The display label of the embedded ole object. |

**Returns:**
byte[] - The byte array data of the embedded ole object .
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Applies the update operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON format string of update operation. |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.String
