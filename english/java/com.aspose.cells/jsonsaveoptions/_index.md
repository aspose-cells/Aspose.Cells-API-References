---
title: JsonSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of saving the workbook as a JSON file.
type: docs
url: /java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

Represents the options of saving the workbook as a JSON file.
## Constructors

| Constructor | Description |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | Creates options for saving json file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getExportArea()](#getExportArea--) | Gets the exporting range. |
| [getExportAsString()](#getExportAsString--) | Exports the string value of the cells to json. |
| [getExportEmptyCells()](#getExportEmptyCells--) | Indicates whether exporting empty cells as null. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | Represents the type of exporting hyperlink to json. |
| [getExportNestedStructure()](#getExportNestedStructure--) | Exported as parent-child hierarchy Json structure. |
| [getExportStylePool()](#getExportStylePool--) | Indicates whether to export styles collectively or individually to each cell. |
| [getIndent()](#getIndent--) | Indicates the indent. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSchemas()](#getSchemas--) | The original json schema of each worksheet. |
| [getSheetIndexes()](#getSheetIndexes--) | Represents the indexes of exported sheets. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | Indicates whether skipping emtpy rows. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getToExcelStruct()](#getToExcelStruct--) | Indicates whether converting to json struct of the Excel file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hasHeaderRow()](#hasHeaderRow--) | Indicates whether the range contains header row. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Sets the exporting range. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exports the string value of the cells to json. |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | Indicates whether exporting empty cells as null. |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | Represents the type of exporting hyperlink to json. |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | Exported as parent-child hierarchy Json structure. |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | Indicates whether to export styles collectively or individually to each cell. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indicates whether the range contains header row. |
| [setIndent(String value)](#setIndent-java.lang.String-) | Indicates the indent. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | The original json schema of each worksheet. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Represents the indexes of exported sheets. |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | Indicates whether skipping emtpy rows. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | Indicates whether converting to json struct of the Excel file. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The folder for temporary files that may be used as data cache.

**Remarks**

If the folder has not been specified, the default value for it is void

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

**Returns:**
boolean
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


If true and the directory does not exist, the directory will be automatically created before saving the file.

**Remarks**

The default value is false.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indicates whether encrypt document properties when saving as .xls file. The default value is true.

**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Gets the exporting range.

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


Represents the type of exporting hyperlink to json.

See [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

The default value is [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


Exported as parent-child hierarchy Json structure.

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


Indicates whether to export styles collectively or individually to each cell.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


Indicates the indent.

**Remarks**

If the indent is null or empty, the exported json is not formatted.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file.

**Remarks**

The default value is false.

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

See [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


The original json schema of each worksheet.

**Returns:**
java.lang.String[]
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


Indicates whether skipping emtpy rows.

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
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


Indicates whether converting to json struct of the Excel file.

**Remarks**

Only for converting range to JSON.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indicates whether updating smart art setting. The default value is false.

**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file.

**Remarks**

The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets warning callback.

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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


The folder for temporary files that may be used as data cache.

**Remarks**

If the folder has not been specified, the default value for it is void

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Make the workbook empty after saving the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


If true and the directory does not exist, the directory will be automatically created before saving the file.

**Remarks**

The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indicates whether encrypt document properties when saving as .xls file. The default value is true.

**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Sets the exporting range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exports the string value of the cells to json.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


Indicates whether exporting empty cells as null.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


Represents the type of exporting hyperlink to json.

See [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

The default value is [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


Exported as parent-child hierarchy Json structure.

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


Indicates whether to export styles collectively or individually to each cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indicates whether the range contains header row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


Indicates the indent.

**Remarks**

If the indent is null or empty, the exported json is not formatted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indicates whether merge the areas of conditional formatting and validation before saving the file.

**Remarks**

The default value is false.

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

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


The original json schema of each worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Represents the indexes of exported sheets.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


Indicates whether skipping emtpy rows.

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

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


Indicates whether converting to json struct of the Excel file.

**Remarks**

Only for converting range to JSON.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indicates whether updating smart art setting. The default value is false.

**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indicates whether validate merged cells before saving the file.

**Remarks**

The default value is false.

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

