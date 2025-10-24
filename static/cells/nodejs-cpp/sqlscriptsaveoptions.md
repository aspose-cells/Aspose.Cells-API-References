##SqlScriptSaveOptions
Represents the options of saving sql.
## SqlScriptSaveOptions class
Represents the options of saving sql.
```javascript
class SqlScriptSaveOptions extends SaveOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving sql file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [checkIfTableExists](#checkIfTableExists--)| boolean | Check if the table name exists before creating |
| [columnTypeMap](#columnTypeMap--)| SqlScriptColumnTypeMap | Gets and sets the map of column type for different database. |
| [checkAllDataForColumnType](#checkAllDataForColumnType--)| boolean | Check all data to find columns' data type. |
| [addBlankLineBetweenRows](#addBlankLineBetweenRows--)| boolean | Insert blank line between each data. |
| [separator](#separator--)| string | Gets and sets character separator of sql script. |
| [operatorType](#operatorType--)| SqlScriptOperatorType | Gets and sets the operator type of sql. |
| [primaryKey](#primaryKey--)| number | Represents which column is primary key of the data table. |
| [createTable](#createTable--)| boolean | Indicates whether exporting sql of creating table. |
| [idName](#idName--)| string | Gets and sets the name of id column. |
| [startId](#startId--)| number | Gets and sets the start id. |
| [tableName](#tableName--)| string | Gets and sets the table name. |
| [exportAsString](#exportAsString--)| boolean | Indicates whether exporting all data as string value. |
| [sheetIndexes](#sheetIndexes--)| number[] | Represents the indexes of exported sheets. |
| [exportArea](#exportArea--)| CellArea | Gets or sets the exporting range. |
| [hasHeaderRow](#hasHeaderRow--)| boolean | Indicates whether the range contains header row. |
| [saveFormat](#saveFormat--)| SaveFormat | Readonly. Gets the save file format. |
| [clearData](#clearData--)| boolean | Make the workbook empty after saving the file. |
| [cachedFileFolder](#cachedFileFolder--)| string | The folder for temporary files that may be used as data cache. |
| [validateMergedAreas](#validateMergedAreas--)| boolean | Indicates whether validate merged cells before saving the file. |
| [mergeAreas](#mergeAreas--)| boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [createDirectory](#createDirectory--)| boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sortNames](#sortNames--)| boolean | Indicates whether sorting defined names before saving file. |
| [sortExternalNames](#sortExternalNames--)| boolean | Indicates whether sorting external defined names before saving file. |
| [refreshChartCache](#refreshChartCache--)| boolean | Indicates whether refreshing chart cache data |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [checkExcelRestriction](#checkExcelRestriction--)| boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [updateSmartArt](#updateSmartArt--)| boolean | Indicates whether updating smart art setting. The default value is false. |
| [encryptDocumentProperties](#encryptDocumentProperties--)| boolean | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
## Methods
| Method | Description |
| --- | --- |
| [getCheckIfTableExists()](#getCheckIfTableExists--)| <b>@deprecated.</b> Please use the 'checkIfTableExists' property instead. Check if the table name exists before creating |
| [setCheckIfTableExists(boolean)](#setCheckIfTableExists-boolean-)| <b>@deprecated.</b> Please use the 'checkIfTableExists' property instead. Check if the table name exists before creating |
| [getColumnTypeMap()](#getColumnTypeMap--)| <b>@deprecated.</b> Please use the 'columnTypeMap' property instead. Gets and sets the map of column type for different database. |
| [setColumnTypeMap(SqlScriptColumnTypeMap)](#setColumnTypeMap-sqlscriptcolumntypemap-)| <b>@deprecated.</b> Please use the 'columnTypeMap' property instead. Gets and sets the map of column type for different database. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--)| <b>@deprecated.</b> Please use the 'checkAllDataForColumnType' property instead. Check all data to find columns' data type. |
| [setCheckAllDataForColumnType(boolean)](#setCheckAllDataForColumnType-boolean-)| <b>@deprecated.</b> Please use the 'checkAllDataForColumnType' property instead. Check all data to find columns' data type. |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--)| <b>@deprecated.</b> Please use the 'addBlankLineBetweenRows' property instead. Insert blank line between each data. |
| [setAddBlankLineBetweenRows(boolean)](#setAddBlankLineBetweenRows-boolean-)| <b>@deprecated.</b> Please use the 'addBlankLineBetweenRows' property instead. Insert blank line between each data. |
| [getSeparator()](#getSeparator--)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets character separator of sql script. |
| [setSeparator(string)](#setSeparator-string-)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets character separator of sql script. |
| [getOperatorType()](#getOperatorType--)| <b>@deprecated.</b> Please use the 'operatorType' property instead. Gets and sets the operator type of sql. |
| [setOperatorType(SqlScriptOperatorType)](#setOperatorType-sqlscriptoperatortype-)| <b>@deprecated.</b> Please use the 'operatorType' property instead. Gets and sets the operator type of sql. |
| [getPrimaryKey()](#getPrimaryKey--)| <b>@deprecated.</b> Please use the 'primaryKey' property instead. Represents which column is primary key of the data table. |
| [setPrimaryKey(number)](#setPrimaryKey-number-)| <b>@deprecated.</b> Please use the 'primaryKey' property instead. Represents which column is primary key of the data table. |
| [getCreateTable()](#getCreateTable--)| <b>@deprecated.</b> Please use the 'createTable' property instead. Indicates whether exporting sql of creating table. |
| [setCreateTable(boolean)](#setCreateTable-boolean-)| <b>@deprecated.</b> Please use the 'createTable' property instead. Indicates whether exporting sql of creating table. |
| [getIdName()](#getIdName--)| <b>@deprecated.</b> Please use the 'idName' property instead. Gets and sets the name of id column. |
| [setIdName(string)](#setIdName-string-)| <b>@deprecated.</b> Please use the 'idName' property instead. Gets and sets the name of id column. |
| [getStartId()](#getStartId--)| <b>@deprecated.</b> Please use the 'startId' property instead. Gets and sets the start id. |
| [setStartId(number)](#setStartId-number-)| <b>@deprecated.</b> Please use the 'startId' property instead. Gets and sets the start id. |
| [getTableName()](#getTableName--)| <b>@deprecated.</b> Please use the 'tableName' property instead. Gets and sets the table name. |
| [setTableName(string)](#setTableName-string-)| <b>@deprecated.</b> Please use the 'tableName' property instead. Gets and sets the table name. |
| [getExportAsString()](#getExportAsString--)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Indicates whether exporting all data as string value. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Indicates whether exporting all data as string value. |
| [getSheetIndexes()](#getSheetIndexes--)| <b>@deprecated.</b> Please use the 'sheetIndexes' property instead. Represents the indexes of exported sheets. |
| [setSheetIndexes(number[])](#setSheetIndexes-numberarray-)| <b>@deprecated.</b> Please use the 'sheetIndexes' property instead. Represents the indexes of exported sheets. |
| [getExportArea()](#getExportArea--)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or sets the exporting range. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or sets the exporting range. |
| [getHasHeaderRow()](#getHasHeaderRow--)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets the save file format. |
| [getClearData()](#getClearData--)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
### constructor() {#constructor--}
Creates options for saving sql file.
```javascript
constructor();
```
### constructor(SaveOptions) {#constructor-saveoptions-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: SaveOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | SaveOptions | The parent object. |
### checkIfTableExists {#checkIfTableExists--}
Check if the table name exists before creating
```javascript
checkIfTableExists : boolean;
```
### columnTypeMap {#columnTypeMap--}
Gets and sets the map of column type for different database.
```javascript
columnTypeMap : SqlScriptColumnTypeMap;
```
### checkAllDataForColumnType {#checkAllDataForColumnType--}
Check all data to find columns' data type.
```javascript
checkAllDataForColumnType : boolean;
```
**Remarks**
The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.
### addBlankLineBetweenRows {#addBlankLineBetweenRows--}
Insert blank line between each data.
```javascript
addBlankLineBetweenRows : boolean;
```
**Remarks**
If [Separator](../separator/) is '\n' , it's better to set this property as true to increase readability.
### separator {#separator--}
Gets and sets character separator of sql script.
```javascript
separator : string;
```
**Remarks**
Only can be ' ' or '\n'. If the
### operatorType {#operatorType--}
Gets and sets the operator type of sql.
```javascript
operatorType : SqlScriptOperatorType;
```
### primaryKey {#primaryKey--}
Represents which column is primary key of the data table.
```javascript
primaryKey : number;
```
### createTable {#createTable--}
Indicates whether exporting sql of creating table.
```javascript
createTable : boolean;
```
### idName {#idName--}
Gets and sets the name of id column.
```javascript
idName : string;
```
**Remarks**
If this property is set , a column will be inserted with automatical increment int value.
### startId {#startId--}
Gets and sets the start id.
```javascript
startId : number;
```
**Remarks**
Only works when [IdName](../idname/) is set.
### tableName {#tableName--}
Gets and sets the table name.
```javascript
tableName : string;
```
### exportAsString {#exportAsString--}
Indicates whether exporting all data as string value.
```javascript
exportAsString : boolean;
```
### sheetIndexes {#sheetIndexes--}
Represents the indexes of exported sheets.
```javascript
sheetIndexes : number[];
```
### exportArea {#exportArea--}
Gets or sets the exporting range.
```javascript
exportArea : CellArea;
```
### hasHeaderRow {#hasHeaderRow--}
Indicates whether the range contains header row.
```javascript
hasHeaderRow : boolean;
```
### saveFormat {#saveFormat--}
Readonly. Gets the save file format.
```javascript
saveFormat : SaveFormat;
```
### clearData {#clearData--}
Make the workbook empty after saving the file.
```javascript
clearData : boolean;
```
### cachedFileFolder {#cachedFileFolder--}
The folder for temporary files that may be used as data cache.
```javascript
cachedFileFolder : string;
```
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### validateMergedAreas {#validateMergedAreas--}
Indicates whether validate merged cells before saving the file.
```javascript
validateMergedAreas : boolean;
```
**Remarks**
The default value is false.
### mergeAreas {#mergeAreas--}
Indicates whether merge the areas of conditional formatting and validation before saving the file.
```javascript
mergeAreas : boolean;
```
**Remarks**
The default value is false.
### createDirectory {#createDirectory--}
If true and the directory does not exist, the directory will be automatically created before saving the file.
```javascript
createDirectory : boolean;
```
**Remarks**
The default value is false.
### sortNames {#sortNames--}
Indicates whether sorting defined names before saving file.
```javascript
sortNames : boolean;
```
### sortExternalNames {#sortExternalNames--}
Indicates whether sorting external defined names before saving file.
```javascript
sortExternalNames : boolean;
```
### refreshChartCache {#refreshChartCache--}
Indicates whether refreshing chart cache data
```javascript
refreshChartCache : boolean;
```
### warningCallback {#warningCallback--}
Gets or sets warning callback.
```javascript
warningCallback : IWarningCallback;
```
### checkExcelRestriction {#checkExcelRestriction--}
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
```javascript
checkExcelRestriction : boolean;
```
### updateSmartArt {#updateSmartArt--}
Indicates whether updating smart art setting. The default value is false.
```javascript
updateSmartArt : boolean;
```
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### encryptDocumentProperties {#encryptDocumentProperties--}
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
```javascript
encryptDocumentProperties : boolean;
```
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
### getCheckIfTableExists() {#getCheckIfTableExists--}
```javascript
getCheckIfTableExists() : boolean;
```
### setCheckIfTableExists(boolean) {#setCheckIfTableExists-boolean-}
```javascript
setCheckIfTableExists(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getColumnTypeMap() {#getColumnTypeMap--}
```javascript
getColumnTypeMap() : SqlScriptColumnTypeMap;
```
**Returns**
[SqlScriptColumnTypeMap](../sqlscriptcolumntypemap/)
### setColumnTypeMap(SqlScriptColumnTypeMap) {#setColumnTypeMap-sqlscriptcolumntypemap-}
```javascript
setColumnTypeMap(value: SqlScriptColumnTypeMap) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../sqlscriptcolumntypemap/) | The value to set. |
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```javascript
getCheckAllDataForColumnType() : boolean;
```
**Remarks**
The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.
### setCheckAllDataForColumnType(boolean) {#setCheckAllDataForColumnType-boolean-}
```javascript
setCheckAllDataForColumnType(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```javascript
getAddBlankLineBetweenRows() : boolean;
```
**Remarks**
If [Separator](../separator/) is '\n' , it's better to set this property as true to increase readability.
### setAddBlankLineBetweenRows(boolean) {#setAddBlankLineBetweenRows-boolean-}
```javascript
setAddBlankLineBetweenRows(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
If [Separator](../separator/) is '\n' , it's better to set this property as true to increase readability.
### getSeparator() {#getSeparator--}
```javascript
getSeparator() : string;
```
**Remarks**
Only can be ' ' or '\n'. If the
### setSeparator(string) {#setSeparator-string-}
```javascript
setSeparator(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Only can be ' ' or '\n'. If the
### getOperatorType() {#getOperatorType--}
```javascript
getOperatorType() : SqlScriptOperatorType;
```
**Returns**
[SqlScriptOperatorType](../sqlscriptoperatortype/)
### setOperatorType(SqlScriptOperatorType) {#setOperatorType-sqlscriptoperatortype-}
```javascript
setOperatorType(value: SqlScriptOperatorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlScriptOperatorType](../sqlscriptoperatortype/) | The value to set. |
### getPrimaryKey() {#getPrimaryKey--}
```javascript
getPrimaryKey() : number;
```
### setPrimaryKey(number) {#setPrimaryKey-number-}
```javascript
setPrimaryKey(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getCreateTable() {#getCreateTable--}
```javascript
getCreateTable() : boolean;
```
### setCreateTable(boolean) {#setCreateTable-boolean-}
```javascript
setCreateTable(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIdName() {#getIdName--}
```javascript
getIdName() : string;
```
**Remarks**
If this property is set , a column will be inserted with automatical increment int value.
### setIdName(string) {#setIdName-string-}
```javascript
setIdName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If this property is set , a column will be inserted with automatical increment int value.
### getStartId() {#getStartId--}
```javascript
getStartId() : number;
```
**Remarks**
Only works when [IdName](../idname/) is set.
### setStartId(number) {#setStartId-number-}
```javascript
setStartId(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Only works when [IdName](../idname/) is set.
### getTableName() {#getTableName--}
```javascript
getTableName() : string;
```
### setTableName(string) {#setTableName-string-}
```javascript
setTableName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getExportAsString() {#getExportAsString--}
```javascript
getExportAsString() : boolean;
```
### setExportAsString(boolean) {#setExportAsString-boolean-}
```javascript
setExportAsString(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSheetIndexes() {#getSheetIndexes--}
```javascript
getSheetIndexes() : number[];
```
**Returns**
number[]
### setSheetIndexes(number[]) {#setSheetIndexes-numberarray-}
```javascript
setSheetIndexes(value: number[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getExportArea() {#getExportArea--}
```javascript
getExportArea() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### setExportArea(CellArea) {#setExportArea-cellarea-}
```javascript
setExportArea(value: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |
### getHasHeaderRow() {#getHasHeaderRow--}
```javascript
getHasHeaderRow() : boolean;
```
### setHasHeaderRow(boolean) {#setHasHeaderRow-boolean-}
```javascript
setHasHeaderRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getSaveFormat() {#getSaveFormat--}
```javascript
getSaveFormat() : SaveFormat;
```
**Returns**
[SaveFormat](../saveformat/)
### getClearData() {#getClearData--}
```javascript
getClearData() : boolean;
```
### setClearData(boolean) {#setClearData-boolean-}
```javascript
setClearData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCachedFileFolder() {#getCachedFileFolder--}
```javascript
getCachedFileFolder() : string;
```
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### setCachedFileFolder(string) {#setCachedFileFolder-string-}
```javascript
setCachedFileFolder(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### getValidateMergedAreas() {#getValidateMergedAreas--}
```javascript
getValidateMergedAreas() : boolean;
```
**Remarks**
The default value is false.
### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}
```javascript
setValidateMergedAreas(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getMergeAreas() {#getMergeAreas--}
```javascript
getMergeAreas() : boolean;
```
**Remarks**
The default value is false.
### setMergeAreas(boolean) {#setMergeAreas-boolean-}
```javascript
setMergeAreas(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getCreateDirectory() {#getCreateDirectory--}
```javascript
getCreateDirectory() : boolean;
```
**Remarks**
The default value is false.
### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}
```javascript
setCreateDirectory(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getSortNames() {#getSortNames--}
```javascript
getSortNames() : boolean;
```
### setSortNames(boolean) {#setSortNames-boolean-}
```javascript
setSortNames(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSortExternalNames() {#getSortExternalNames--}
```javascript
getSortExternalNames() : boolean;
```
### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}
```javascript
setSortExternalNames(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshChartCache() {#getRefreshChartCache--}
```javascript
getRefreshChartCache() : boolean;
```
### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}
```javascript
setRefreshChartCache(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}
```javascript
setWarningCallback(value: IWarningCallback) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |
### getWarningCallback() {#getWarningCallback--}
```javascript
getWarningCallback() : IWarningCallback;
```
**Returns**
[IWarningCallback](../iwarningcallback/)
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```javascript
getCheckExcelRestriction() : boolean;
```
### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}
```javascript
setCheckExcelRestriction(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getUpdateSmartArt() {#getUpdateSmartArt--}
```javascript
getUpdateSmartArt() : boolean;
```
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}
```javascript
setUpdateSmartArt(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```javascript
getEncryptDocumentProperties() : boolean;
```
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}
```javascript
setEncryptDocumentProperties(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
