---
title: XmlSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of saving the workbook as an xml file.
type: docs
weight: 671
url: /java/com.aspose.cells/xmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class XmlSaveOptions extends SaveOptions
```

Represents the options of saving the workbook as an xml file.
## Constructors

| Constructor | Description |
| --- | --- |
| [XmlSaveOptions()](#XmlSaveOptions--) | Creates options for saving xml file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getExportArea()](#getExportArea--) | Gets or sets the exporting range. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSheetIndexes()](#getSheetIndexes--) | Represents the indexes of exported sheets. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [getXmlMapName()](#getXmlMapName--) | Indicates whether exporting xml map in the file. |
| [hasHeaderRow()](#hasHeaderRow--) | Indicates whether the range contains header row. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--) |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--) |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--) |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | For the description of this property, please see [getExportArea()](../../com.aspose.cells/xmlsaveoptions\#getExportArea--) |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | For the description of this property, please see [hasHeaderRow()](../../com.aspose.cells/xmlsaveoptions\#hasHeaderRow--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--) |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | For the description of this property, please see [getSheetIndexes()](../../com.aspose.cells/xmlsaveoptions\#getSheetIndexes--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--) |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--) |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [setXmlMapName(String value)](#setXmlMapName-java.lang.String-) | For the description of this property, please see [getXmlMapName()](../../com.aspose.cells/xmlsaveoptions\#getXmlMapName--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlSaveOptions() {#XmlSaveOptions--}
```
public XmlSaveOptions()
```


Creates options for saving xml file.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Gets or sets the exporting range.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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


Gets the save file format.

**Returns:**
int
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Represents the indexes of exported sheets.

**Returns:**
int[]
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


Gets or sets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getXmlMapName() {#getXmlMapName--}
```
public String getXmlMapName()
```


Indicates whether exporting xml map in the file.

**Returns:**
java.lang.String
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Indicates whether the range contains header row.

**Returns:**
boolean
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


For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


For the description of this property, please see [getExportArea()](../../com.aspose.cells/xmlsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


For the description of this property, please see [hasHeaderRow()](../../com.aspose.cells/xmlsaveoptions\#hasHeaderRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


For the description of this property, please see [getSheetIndexes()](../../com.aspose.cells/xmlsaveoptions\#getSheetIndexes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setXmlMapName(String value) {#setXmlMapName-java.lang.String-}
```
public void setXmlMapName(String value)
```


For the description of this property, please see [getXmlMapName()](../../com.aspose.cells/xmlsaveoptions\#getXmlMapName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

