---
title: GridJsWorkbook
second_title: Aspose.Cells for Java API Reference
description: Represents the main entry class for GridJs
type: docs
url: /java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Represents the main entry class for GridJs
## Constructors

| Constructor | Description |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) |  |
## Fields

| Field | Description |
| --- | --- |
| [CacheImp](#CacheImp) | Custom implemention for cache storage,If you want to store cache in stream way ,you need to set and implement it. |
| [CalculateEngine](#CalculateEngine) | Custom implemention for calculation engine ,If you want to do custom calculation, you need to set and implement it. |
| [PICTURE_TYPE](#PICTURE-TYPE) | const value for the type of the image |
| [UpdateMonitor](#UpdateMonitor) | Gets/Sets the update monitor to track update operation |
## Methods

| Method | Description |
| --- | --- |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only. |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Copys image or shape. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Gets the error message string in JSON format. |
| [exportToJson()](#exportToJson--) | Gets JSON string from memory data, the default filename in the JSON is: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Gets JSON string from memory data,set the output filename in the JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Gets JSON string from memory data,set the output filename in the JSON. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Gets the load format by file extension |
| [getImageStream(String uid, String picid)](#getImageStream-java.lang.String-java.lang.String-) | Get Stream of image. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Gets the image URL. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Gets the byte array data of the embedded ole object . |
| [getSettings()](#getSettings--) | Represents the workbook settings. |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Generates a new unique id for the file cache using the given file name. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Imports the excel file from file stream with load format. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Imports the excel file from file stream with load format and open password. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Imports the excel file from the file path. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Imports the excel file from file stream. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Imports the excel file from file stream with load format and open password. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Imports the excel file from the file path. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Imports the excel file from file path and open password. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Imports the excel file from JSON format string. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Inserts image in the worksheet from file stream or the URL,(either the file stream or the URL shall be provided) or Inserts shape ,when the p.type is one of AutoShapeType |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Retrieve the JSON string from memory data,set the output filename in the JSON, and write it to the stream. |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Retrieve the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON,and write it to the stream. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Gets the JSON string of the specified sheet in the file from the cache using the specified unique id. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Retrieve the JSON string of the specified sheet in the file from the cache using the specified unique id, and write it to the stream. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Applies a batch update to the memory data. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Saves the memory data to the cache file with the specified filename and also set the open password, the save format is baseed on the file extension of the filename . |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Saves the memory data to the sream, baseed on the origin file format. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Saves the memory data to the file path,if the file has extension ,save format is baseed on the file extension . |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Saves the memory data to the sream,the save format is html |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Saves the memory data to the file path,the save format is html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Saves the memory data to the sream,the save format is pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Saves the memory data to the file path,the save format is pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Saves the memory data to the sream,the save format is xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Saves the memory data to the file path,the save format is xlsx. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Set the base image get action URL from controller . |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Sets InterruptMonitor for load operation. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Sets InterruptMonitor for save operation. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Represents the workbook settings. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Translate all the string value to the target language in the worksheet |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applies the update operation. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Custom implemention for cache storage,If you want to store cache in stream way ,you need to set and implement it.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Custom implemention for calculation engine ,If you want to do custom calculation, you need to set and implement it.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


const value for the type of the image

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Gets/Sets the update monitor to track update operation

### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Check wether workbook instance is in memory cache .this method is apply for Collaborative mode only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean - 
### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Copys image or shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| p | java.lang.String | The JSON string for the operation which specify the cell location ,it contains the worksheet name,upper left row,upper left column for the image or shape\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - The JSON string of the new copied image
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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Gets the error message string in JSON format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| msg | java.lang.String | The error message. |

**Returns:**
java.lang.String - The JSON string.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Gets JSON string from memory data, the default filename in the JSON is: book1.

**Returns:**
java.lang.String - The JSON string.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Gets JSON string from memory data,set the output filename in the JSON.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1.. |

**Returns:**
java.lang.String - The JSON string.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Gets JSON string from memory data,set the output filename in the JSON.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1.. |

**Returns:**
java.lang.StringBuilder - The JSON StringBuilder.
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


Gets the load format by file extension

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | java.lang.String | The file extention ,usually start with '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid) {#getImageStream-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid)
```


Get Stream of image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| picid | java.lang.String | The image id. |

**Returns:**
java.io.InputStream - The image stream
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Gets the image URL.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| picid | java.lang.String | The image id. |
| delimiter | java.lang.String | The string delimiter. |

**Returns:**
java.lang.String - 
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Gets the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |

**Returns:**
java.lang.StringBuilder - The JSON string StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Represents the workbook settings.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Generates a new unique id for the file cache using the given file name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

**Returns:**
java.lang.String - 
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


Imports the excel file from file stream with load format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filestream | java.io.InputStream | The stream of the excel file . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). The LoadFormat of the excel file. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Imports the excel file from file stream with load format and open password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filestream | java.io.InputStream | The stream of the excel file . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). The LoadFormat of the excel file. |
| password | java.lang.String | The open password of the excel file.The value can be null If no passowrd is set. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Imports the excel file from the file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full path of the file. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Imports the excel file from file stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache, if set to null,it will be generated automatically. |
| filestream | java.io.InputStream | The stream of the excel file . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). The LoadFormat of the excel file. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Imports the excel file from file stream with load format and open password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache, if set to null,it will be generated automatically. |
| filestream | java.io.InputStream | The stream of the excel file . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). The LoadFormat of the excel file. |
| password | java.lang.String | The open password of the excel file.The value can be null If no passowrd is set |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Imports the excel file from the file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache, if set to null,it will be generated automatically. |
| fileName | java.lang.String | The full path of the file. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Imports the excel file from file path and open password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache, if set to null,it will be generated automatically. |
| fileName | java.lang.String | The full path of the file. |
| password | java.lang.String | The open password of the excel file.The value can be null If no passowrd is set. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Imports the excel file from JSON format string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| json | java.lang.String | The JSON format string. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Inserts image in the worksheet from file stream or the URL,(either the file stream or the URL shall be provided) or Inserts shape ,when the p.type is one of AutoShapeType

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache |
| p | java.lang.String | The JSON format string for the operation which specify the cell location ,the worksheet name,upper left row,upper left column for the image\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | The file stream of the image file |
| imageUrl | java.lang.String | The URL of the image file |

**Returns:**
java.lang.String - The JSON format string of the inserted image
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Retrieve the JSON string from memory data,set the output filename in the JSON, and write it to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Retrieve the JSON string of the file from the cache using the specified unique id,set the output filename in the JSON,and write it to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| uid | java.lang.String | The unique id for the file cache. |
| filename | java.lang.String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Gets the JSON string of the specified sheet in the file from the cache using the specified unique id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| sheetName | java.lang.String | the sheet name. |

**Returns:**
java.lang.StringBuilder - The JSON string StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Retrieve the JSON string of the specified sheet in the file from the cache using the specified unique id, and write it to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream that will be written |
| uid | java.lang.String | The unique id for the file cache. |
| sheetName | java.lang.String | the sheet name. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Applies a batch update to the memory data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| json | java.lang.String | The update JSON format string. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Saves the memory data to the cache file with the specified filename and also set the open password, the save format is baseed on the file extension of the filename .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| filename | java.lang.String | The filename to save. |
| password | java.lang.String | The excel file's open password. The value can be null If no passowrd is set. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Saves the memory data to the sream, baseed on the origin file format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Saves the memory data to the file path,if the file has extension ,save format is baseed on the file extension .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The file path to save. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Saves the memory data to the sream,the save format is html

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Saves the memory data to the file path,the save format is html.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The file path to save. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Saves the memory data to the sream,the save format is pdf.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Saves the memory data to the file path,the save format is pdf.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The file path to save. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Saves the memory data to the sream,the save format is xlsx.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Saves the memory data to the file path,the save format is xlsx.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The file path to save. |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Set the base image get action URL from controller .

**Remarks**

when CacheImp is null,we need to set this .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseImageURL | java.lang.String | the base image get action URL. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Sets InterruptMonitor for load operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | The InterruptMonitor instance. |
| calculateTimeoutMilliseconds | int | The time out in millisecond for load file. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Sets InterruptMonitor for save operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | The InterruptMonitor instance. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Represents the workbook settings.

**Parameters:**
| Parameter | Type | Description |
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


Translate all the string value to the target language in the worksheet

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
| sheetName | java.lang.String | The sheet name |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | The translator which implement translate function |
| targetLanguage | java.lang.String | The target language |

**Returns:**
java.lang.String - 
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Applies the update operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | java.lang.String | The JSON format string of update operation. |
| uid | java.lang.String | The unique id for the file cache. |

**Returns:**
java.lang.String - The JSON format string of the update result.
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

