---
title: SqlScriptSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of saving sql.
type: docs
weight: 549
url: /java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

Represents the options of saving sql.
## Constructors

| Constructor | Description |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | Creates options for saving sql file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | Insert blank line between each data. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | Check all data to find columns' data type. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | Check if the table name exists before creating |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getColumnTypeMap()](#getColumnTypeMap--) | Gets and sets the map of column type for different database. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getCreateTable()](#getCreateTable--) | Indicates whether exporting sql of creating table. |
| [getExportArea()](#getExportArea--) | Gets or sets the exporting range. |
| [getExportAsString()](#getExportAsString--) | Indicates whether exporting all data as string value. |
| [getIdName()](#getIdName--) | Gets and sets the name of id column. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getOperatorType()](#getOperatorType--) | Gets and sets the operator type of sql. |
| [getPrimaryKey()](#getPrimaryKey--) | Represents which column is primary key of the data table. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSeparator()](#getSeparator--) | Gets and sets character separator of sql script. |
| [getSheetIndexes()](#getSheetIndexes--) | Represents the indexes of exported sheets. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getStartId()](#getStartId--) | Gets and sets the start id. |
| [getTableName()](#getTableName--) | Gets and sets the table name. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [hasHeaderRow()](#hasHeaderRow--) | Indicates whether the range contains header row. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | For the description of this property, please see \#getAddBlankLineBetweenRows().getAddBlankLineBetweenRows() |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see \#getCachedFileFolder().getCachedFileFolder() |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | For the description of this property, please see \#getCheckAllDataForColumnType().getCheckAllDataForColumnType() |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | For the description of this property, please see \#getCheckIfTableExists().getCheckIfTableExists() |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see \#getClearData().getClearData() |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | For the description of this property, please see \#getColumnTypeMap().getColumnTypeMap() |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see \#getCreateDirectory().getCreateDirectory() |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | For the description of this property, please see \#getCreateTable().getCreateTable() |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | For the description of this property, please see \#getExportArea().getExportArea() |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | For the description of this property, please see \#getExportAsString().getExportAsString() |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | For the description of this property, please see \#hasHeaderRow().hasHeaderRow() |
| [setIdName(String value)](#setIdName-java.lang.String-) | For the description of this property, please see \#getIdName().getIdName() |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see \#getMergeAreas().getMergeAreas() |
| [setOperatorType(int value)](#setOperatorType-int-) | For the description of this property, please see \#getOperatorType().getOperatorType() |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | For the description of this property, please see \#getPrimaryKey().getPrimaryKey() |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see \#getRefreshChartCache().getRefreshChartCache() |
| [setSeparator(char value)](#setSeparator-char-) | For the description of this property, please see \#getSeparator().getSeparator() |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | For the description of this property, please see \#getSheetIndexes().getSheetIndexes() |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | For the description of this property, please see \#getSortExternalNames().getSortExternalNames() |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see \#getSortNames().getSortNames() |
| [setStartId(int value)](#setStartId-int-) | For the description of this property, please see \#getStartId().getStartId() |
| [setTableName(String value)](#setTableName-java.lang.String-) | For the description of this property, please see \#getTableName().getTableName() |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | For the description of this property, please see \#getUpdateSmartArt().getUpdateSmartArt() |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see \#getValidateMergedAreas().getValidateMergedAreas() |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


Creates options for saving sql file.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


Insert blank line between each data. If [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) is '\\n' , it's better to set this property as true to increase readability.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The cached file folder is used to store some large data.

**Returns:**
java.lang.String
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


Check all data to find columns' data type. The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


Check if the table name exists before creating

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
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


Gets and sets the map of column type for different database.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


Indicates whether exporting sql of creating table.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Gets or sets the exporting range.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Indicates whether exporting all data as string value.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int value.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Returns:**
boolean
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


Gets and sets the operator type of sql.

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


Represents which column is primary key of the data table.

**Returns:**
int
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Gets and sets character separator of sql script. Only can be ' ' or '\\n'. If the

**Returns:**
char
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
### getStartId() {#getStartId--}
```
public int getStartId()
```


Gets and sets the start id. Only works when [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) is set.

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


Gets and sets the table name.

**Returns:**
java.lang.String
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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


For the description of this property, please see \#getAddBlankLineBetweenRows().getAddBlankLineBetweenRows()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


For the description of this property, please see \#getCachedFileFolder().getCachedFileFolder()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


For the description of this property, please see \#getCheckAllDataForColumnType().getCheckAllDataForColumnType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


For the description of this property, please see \#getCheckIfTableExists().getCheckIfTableExists()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


For the description of this property, please see \#getClearData().getClearData()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


For the description of this property, please see \#getColumnTypeMap().getColumnTypeMap()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


For the description of this property, please see \#getCreateDirectory().getCreateDirectory()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


For the description of this property, please see \#getCreateTable().getCreateTable()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


For the description of this property, please see \#getExportArea().getExportArea()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


For the description of this property, please see \#getExportAsString().getExportAsString()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


For the description of this property, please see \#hasHeaderRow().hasHeaderRow()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


For the description of this property, please see \#getIdName().getIdName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


For the description of this property, please see \#getMergeAreas().getMergeAreas()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


For the description of this property, please see \#getOperatorType().getOperatorType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


For the description of this property, please see \#getPrimaryKey().getPrimaryKey()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


For the description of this property, please see \#getRefreshChartCache().getRefreshChartCache()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


For the description of this property, please see \#getSeparator().getSeparator()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


For the description of this property, please see \#getSheetIndexes().getSheetIndexes()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


For the description of this property, please see \#getSortExternalNames().getSortExternalNames()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


For the description of this property, please see \#getSortNames().getSortNames()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


For the description of this property, please see \#getStartId().getStartId()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


For the description of this property, please see \#getTableName().getTableName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


For the description of this property, please see \#getUpdateSmartArt().getUpdateSmartArt()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


For the description of this property, please see \#getValidateMergedAreas().getValidateMergedAreas()

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

