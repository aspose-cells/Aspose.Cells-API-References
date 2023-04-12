---
title: OoxmlSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of saving office open xml file.
type: docs
url: /java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Represents the options of saving office open xml file.
## Constructors

| Constructor | Description |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Creates the options for saving office open xml file. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Creates the options for saving office open xml file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCompressionType()](#getCompressionType--) | Gets the compression type for ooxml file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [getEnableZip64()](#getEnableZip64--) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [getExportCellName()](#getExportCellName--) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | The data provider for saving workbook in light mode. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getUpdateZoom()](#getUpdateZoom--) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The cached file folder is used to store some large data. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCompressionType(int value)](#setCompressionType-int-) | Sets the compression type for ooxml file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | The data provider for saving workbook in light mode. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Creates the options for saving office open xml file.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Creates the options for saving office open xml file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). The file format. It must be xlsx,xltx,xlsm,xltm. |

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The cached file folder is used to store some large data.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Make the workbook empty after saving the file.

**Returns:**
boolean
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Gets the compression type for ooxml file. [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype). The default value is OoxmlCompressionType.Level2.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Always use ZIP64 extensions when writing zip archives, even when unnecessary.

**Returns:**
boolean
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


The data provider for saving workbook in light mode.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indicates whether refreshing chart cache data

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the save file format. [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indicates whether sorting external defined names before saving file.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indicates whether sorting defined names before saving file.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Returns:**
boolean
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. The default value is false for performance.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file. The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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




### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


The cached file folder is used to store some large data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Make the workbook empty after saving the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Sets the compression type for ooxml file. [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype). The default value is OoxmlCompressionType.Level2.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Always use ZIP64 extensions when writing zip archives, even when unnecessary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


The data provider for saving workbook in light mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indicates whether refreshing chart cache data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indicates whether sorting external defined names before saving file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indicates whether sorting defined names before saving file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. The default value is false for performance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indicates whether validate merged cells before saving the file. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Sets warning callback.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

