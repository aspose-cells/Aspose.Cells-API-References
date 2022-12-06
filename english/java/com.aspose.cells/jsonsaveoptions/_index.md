---
title: JsonSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of saving the workbook as a json file.
type: docs
url: /java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

Represents the options of saving the workbook as a json file.
## Constructors

| Constructor | Description |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | Creates options for saving json file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getExportArea()](#getExportArea--) | the exporting range. |
| [getExportAsString()](#getExportAsString--) | Exports the string value of the cells to json. |
| [getExportEmptyCells()](#getExportEmptyCells--) | Indicates whether exporting empty cells as null. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | Represents the type of exporting hyperlink to json. |
| [getExportNestedStructure()](#getExportNestedStructure--) | Exported as parent-child hierarchy Json structure. |
| [getIndent()](#getIndent--) | Indicates the indent. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSheetIndexes()](#getSheetIndexes--) | Represents the indexes of exported sheets. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | Indicates whether skpping emtpy rows |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | warning callback. |
| [hasHeaderRow()](#hasHeaderRow--) | Indicates whether the range contains header row. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--) |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--) |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--) |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | For the description of this property, please see [getExportArea()](../../com.aspose.cells/jsonsaveoptions\#getExportArea--) |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | For the description of this property, please see [getExportAsString()](../../com.aspose.cells/jsonsaveoptions\#getExportAsString--) |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | For the description of this property, please see [getExportEmptyCells()](../../com.aspose.cells/jsonsaveoptions\#getExportEmptyCells--) |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | For the description of this property, please see [getExportHyperlinkType()](../../com.aspose.cells/jsonsaveoptions\#getExportHyperlinkType--) |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | For the description of this property, please see [getExportNestedStructure()](../../com.aspose.cells/jsonsaveoptions\#getExportNestedStructure--) |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | For the description of this property, please see [hasHeaderRow()](../../com.aspose.cells/jsonsaveoptions\#hasHeaderRow--) |
| [setIndent(String value)](#setIndent-java.lang.String-) | For the description of this property, please see [getIndent()](../../com.aspose.cells/jsonsaveoptions\#getIndent--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--) |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | For the description of this property, please see [getSheetIndexes()](../../com.aspose.cells/jsonsaveoptions\#getSheetIndexes--) |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | For the description of this property, please see [getSkipEmptyRows()](../../com.aspose.cells/jsonsaveoptions\#getSkipEmptyRows--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--) |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--) |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


Creates options for saving json file.

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


the exporting range.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exports the string value of the cells to json.

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


Indicates whether exporting empty cells as null.

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


Represents the type of exporting hyperlink to json. The default value is JsonExportHyperlinkType.DISPLAY\_STRING;

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


Exported as parent-child hierarchy Json structure.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


Indicates the indent. If the indent is null or empty, the exported json is not formatted.

**Returns:**
java.lang.String
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
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


Indicates whether skpping emtpy rows

**Returns:**
boolean
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


warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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


For the description of this property, please see [getExportArea()](../../com.aspose.cells/jsonsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


For the description of this property, please see [getExportAsString()](../../com.aspose.cells/jsonsaveoptions\#getExportAsString--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


For the description of this property, please see [getExportEmptyCells()](../../com.aspose.cells/jsonsaveoptions\#getExportEmptyCells--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


For the description of this property, please see [getExportHyperlinkType()](../../com.aspose.cells/jsonsaveoptions\#getExportHyperlinkType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


For the description of this property, please see [getExportNestedStructure()](../../com.aspose.cells/jsonsaveoptions\#getExportNestedStructure--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


For the description of this property, please see [hasHeaderRow()](../../com.aspose.cells/jsonsaveoptions\#hasHeaderRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


For the description of this property, please see [getIndent()](../../com.aspose.cells/jsonsaveoptions\#getIndent--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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


For the description of this property, please see [getSheetIndexes()](../../com.aspose.cells/jsonsaveoptions\#getSheetIndexes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


For the description of this property, please see [getSkipEmptyRows()](../../com.aspose.cells/jsonsaveoptions\#getSkipEmptyRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

