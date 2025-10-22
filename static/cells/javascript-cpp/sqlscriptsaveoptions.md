##SqlScriptSaveOptions
Represents the options of saving sql.
## SqlScriptSaveOptions class
Represents the options of saving sql.
```javascript
class SqlScriptSaveOptions extends SaveOptions;
```
## Constructors
| Name | Description |
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
