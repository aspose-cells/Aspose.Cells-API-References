---
title: "SqlScriptSaveOptions"
linktitle: "SqlScriptSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options of saving sql."
type: docs
weight: 3930
url: /nodejs/aspose.cells/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Represents the options of saving sql.

```js
new SqlScriptSaveOptions()
```

Creates options for saving sql file.

## Methods

| Name | Description |
| --- | --- |
| [getAddBlankLineBetweenRows()](#getaddblanklinebetweenrows) | Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readabi |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckAllDataForColumnType()](#getcheckalldataforcolumntype) | Check all data to find columns' data type. The default value is false, we only check the first row for performance. If t |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getCheckIfTableExists()](#getcheckiftableexists) | Check if the table name exists before creating |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getColumnTypeMap()](#getcolumntypemap) | Gets and sets the map of column type for different database. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getCreateTable()](#getcreatetable) | Indicates whether exporting sql of creating table. |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExportArea()](#getexportarea) | Gets or sets the exporting range. |
| [getExportAsString()](#getexportasstring) | Indicates whether exporting all data as string value. |
| [getIdName()](#getidname) | Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int  |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getOperatorType()](#getoperatortype) | Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant. |
| [getPrimaryKey()](#getprimarykey) | Represents which column is primary key of the data table. |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSeparator()](#getseparator) | Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the |
| [getSheetIndexes()](#getsheetindexes) | Represents the indexes of exported sheets. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getStartId()](#getstartid) | Gets and sets the start id. Only works when IdName is set. |
| [getTableName()](#gettablename) | Gets and sets the table name. |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWarningCallback()](#getwarningcallback) | Gets or sets warning callback. |
| [hasHeaderRow()](#hasheaderrow) | Indicates whether the range contains header row. |
| [setAddBlankLineBetweenRows()](#setaddblanklinebetweenrows) | Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readabi |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckAllDataForColumnType()](#setcheckalldataforcolumntype) | Check all data to find columns' data type. The default value is false, we only check the first row for performance. If t |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setCheckIfTableExists()](#setcheckiftableexists) | Check if the table name exists before creating |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setColumnTypeMap()](#setcolumntypemap) | Gets and sets the map of column type for different database. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setCreateTable()](#setcreatetable) | Indicates whether exporting sql of creating table. |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExportArea()](#setexportarea) | Gets or sets the exporting range. |
| [setExportAsString()](#setexportasstring) | Indicates whether exporting all data as string value. |
| [setHasHeaderRow()](#sethasheaderrow) | Indicates whether the range contains header row. |
| [setIdName()](#setidname) | Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int  |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setOperatorType()](#setoperatortype) | Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant. |
| [setPrimaryKey()](#setprimarykey) | Represents which column is primary key of the data table. |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSeparator()](#setseparator) | Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the |
| [setSheetIndexes()](#setsheetindexes) | Represents the indexes of exported sheets. |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setStartId()](#setstartid) | Gets and sets the start id. Only works when IdName is set. |
| [setTableName()](#settablename) | Gets and sets the table name. |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWarningCallback()](#setwarningcallback) | Gets or sets warning callback. |

### getAddBlankLineBetweenRows() {#getaddblanklinebetweenrows}

Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readability.

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCheckAllDataForColumnType() {#getcheckalldataforcolumntype}

Check all data to find columns' data type. The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getCheckIfTableExists() {#getcheckiftableexists}

Check if the table name exists before creating

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getColumnTypeMap() {#getcolumntypemap}

Gets and sets the map of column type for different database.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getCreateTable() {#getcreatetable}

Indicates whether exporting sql of creating table.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExportArea() {#getexportarea}

Gets or sets the exporting range.

### getExportAsString() {#getexportasstring}

Indicates whether exporting all data as string value.

### getIdName() {#getidname}

Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int value.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getOperatorType() {#getoperatortype}

Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant.

### getPrimaryKey() {#getprimarykey}

Represents which column is primary key of the data table.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSeparator() {#getseparator}

Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the

### getSheetIndexes() {#getsheetindexes}

Represents the indexes of exported sheets.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getStartId() {#getstartid}

Gets and sets the start id. Only works when IdName is set.

### getTableName() {#gettablename}

Gets and sets the table name.

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWarningCallback() {#getwarningcallback}

Gets or sets warning callback.

### hasHeaderRow() {#hasheaderrow}

Indicates whether the range contains header row.

### setAddBlankLineBetweenRows() {#setaddblanklinebetweenrows}

Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readability.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckAllDataForColumnType() {#setcheckalldataforcolumntype}

Check all data to find columns' data type. The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setCheckIfTableExists() {#setcheckiftableexists}

Check if the table name exists before creating

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setColumnTypeMap() {#setcolumntypemap}

Gets and sets the map of column type for different database.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setCreateTable() {#setcreatetable}

Indicates whether exporting sql of creating table.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExportArea() {#setexportarea}

Gets or sets the exporting range.

### setExportAsString() {#setexportasstring}

Indicates whether exporting all data as string value.

### setHasHeaderRow() {#sethasheaderrow}

Indicates whether the range contains header row.

### setIdName() {#setidname}

Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int value.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setOperatorType() {#setoperatortype}

Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant.

### setPrimaryKey() {#setprimarykey}

Represents which column is primary key of the data table.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSeparator() {#setseparator}

Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the

### setSheetIndexes() {#setsheetindexes}

Represents the indexes of exported sheets.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setStartId() {#setstartid}

Gets and sets the start id. Only works when IdName is set.

### setTableName() {#settablename}

Gets and sets the table name.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWarningCallback() {#setwarningcallback}

Gets or sets warning callback.
