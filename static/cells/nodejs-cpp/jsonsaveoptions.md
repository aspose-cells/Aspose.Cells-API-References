##JsonSaveOptions
Represents the options of saving the workbook as a json file.
## JsonSaveOptions class
Represents the options of saving the workbook as a json file.
```javascript
class JsonSaveOptions extends SaveOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving json file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [exportStylePool](#exportStylePool--)| boolean | Indicates whether to export styles collectively or individually to each cell. |
| [exportHyperlinkType](#exportHyperlinkType--)| JsonExportHyperlinkType | Represents the type of exporting hyperlink to json. |
| [skipEmptyRows](#skipEmptyRows--)| boolean | Indicates whether skipping emtpy rows. |
| [sheetIndexes](#sheetIndexes--)| number[] | Represents the indexes of exported sheets. |
| [schemas](#schemas--)| string[] | The original json schema of each worksheet. |
| [exportArea](#exportArea--)| CellArea | Gets or sets the exporting range. |
| [hasHeaderRow](#hasHeaderRow--)| boolean | Indicates whether the range contains header row. |
| [exportAsString](#exportAsString--)| boolean | Exports the string value of the cells to json. |
| [indent](#indent--)| string | Indicates the indent. |
| [exportNestedStructure](#exportNestedStructure--)| boolean | Exported as parent-child hierarchy Json structure. |
| [exportEmptyCells](#exportEmptyCells--)| boolean | Indicates whether exporting empty cells as null. |
| [alwaysExportAsJsonObject](#alwaysExportAsJsonObject--)| boolean | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [toExcelStruct](#toExcelStruct--)| boolean | Indicates whether converting to json struct of the Excel file. |
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
| [getExportStylePool()](#getExportStylePool--)| <b>@deprecated.</b> Please use the 'exportStylePool' property instead. Indicates whether to export styles collectively or individually to each cell. |
| [setExportStylePool(boolean)](#setExportStylePool-boolean-)| <b>@deprecated.</b> Please use the 'exportStylePool' property instead. Indicates whether to export styles collectively or individually to each cell. |
| [getExportHyperlinkType()](#getExportHyperlinkType--)| <b>@deprecated.</b> Please use the 'exportHyperlinkType' property instead. Represents the type of exporting hyperlink to json. |
| [setExportHyperlinkType(JsonExportHyperlinkType)](#setExportHyperlinkType-jsonexporthyperlinktype-)| <b>@deprecated.</b> Please use the 'exportHyperlinkType' property instead. Represents the type of exporting hyperlink to json. |
| [getSkipEmptyRows()](#getSkipEmptyRows--)| <b>@deprecated.</b> Please use the 'skipEmptyRows' property instead. Indicates whether skipping emtpy rows. |
| [setSkipEmptyRows(boolean)](#setSkipEmptyRows-boolean-)| <b>@deprecated.</b> Please use the 'skipEmptyRows' property instead. Indicates whether skipping emtpy rows. |
| [getSheetIndexes()](#getSheetIndexes--)| <b>@deprecated.</b> Please use the 'sheetIndexes' property instead. Represents the indexes of exported sheets. |
| [setSheetIndexes(number[])](#setSheetIndexes-numberarray-)| <b>@deprecated.</b> Please use the 'sheetIndexes' property instead. Represents the indexes of exported sheets. |
| [getSchemas()](#getSchemas--)| <b>@deprecated.</b> Please use the 'schemas' property instead. The original json schema of each worksheet. |
| [setSchemas(string[])](#setSchemas-stringarray-)| <b>@deprecated.</b> Please use the 'schemas' property instead. The original json schema of each worksheet. |
| [getExportArea()](#getExportArea--)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or sets the exporting range. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or sets the exporting range. |
| [getHasHeaderRow()](#getHasHeaderRow--)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [getExportAsString()](#getExportAsString--)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Exports the string value of the cells to json. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Exports the string value of the cells to json. |
| [getIndent()](#getIndent--)| <b>@deprecated.</b> Please use the 'indent' property instead. Indicates the indent. |
| [setIndent(string)](#setIndent-string-)| <b>@deprecated.</b> Please use the 'indent' property instead. Indicates the indent. |
| [getExportNestedStructure()](#getExportNestedStructure--)| <b>@deprecated.</b> Please use the 'exportNestedStructure' property instead. Exported as parent-child hierarchy Json structure. |
| [setExportNestedStructure(boolean)](#setExportNestedStructure-boolean-)| <b>@deprecated.</b> Please use the 'exportNestedStructure' property instead. Exported as parent-child hierarchy Json structure. |
| [getExportEmptyCells()](#getExportEmptyCells--)| <b>@deprecated.</b> Please use the 'exportEmptyCells' property instead. Indicates whether exporting empty cells as null. |
| [setExportEmptyCells(boolean)](#setExportEmptyCells-boolean-)| <b>@deprecated.</b> Please use the 'exportEmptyCells' property instead. Indicates whether exporting empty cells as null. |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--)| <b>@deprecated.</b> Please use the 'alwaysExportAsJsonObject' property instead. Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [setAlwaysExportAsJsonObject(boolean)](#setAlwaysExportAsJsonObject-boolean-)| <b>@deprecated.</b> Please use the 'alwaysExportAsJsonObject' property instead. Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [getToExcelStruct()](#getToExcelStruct--)| <b>@deprecated.</b> Please use the 'toExcelStruct' property instead. Indicates whether converting to json struct of the Excel file. |
| [setToExcelStruct(boolean)](#setToExcelStruct-boolean-)| <b>@deprecated.</b> Please use the 'toExcelStruct' property instead. Indicates whether converting to json struct of the Excel file. |
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
Creates options for saving json file.
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
### exportStylePool {#exportStylePool--}
Indicates whether to export styles collectively or individually to each cell.
```javascript
exportStylePool : boolean;
```
### exportHyperlinkType {#exportHyperlinkType--}
Represents the type of exporting hyperlink to json.
```javascript
exportHyperlinkType : JsonExportHyperlinkType;
```
**Remarks**
The default value is [JsonExportHyperlinkType.DisplayString](../jsonexporthyperlinktype.displaystring/);
### skipEmptyRows {#skipEmptyRows--}
Indicates whether skipping emtpy rows.
```javascript
skipEmptyRows : boolean;
```
### sheetIndexes {#sheetIndexes--}
Represents the indexes of exported sheets.
```javascript
sheetIndexes : number[];
```
### schemas {#schemas--}
The original json schema of each worksheet.
```javascript
schemas : string[];
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
### exportAsString {#exportAsString--}
Exports the string value of the cells to json.
```javascript
exportAsString : boolean;
```
### indent {#indent--}
Indicates the indent.
```javascript
indent : string;
```
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### exportNestedStructure {#exportNestedStructure--}
Exported as parent-child hierarchy Json structure.
```javascript
exportNestedStructure : boolean;
```
### exportEmptyCells {#exportEmptyCells--}
Indicates whether exporting empty cells as null.
```javascript
exportEmptyCells : boolean;
```
### alwaysExportAsJsonObject {#alwaysExportAsJsonObject--}
Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.
```javascript
alwaysExportAsJsonObject : boolean;
```
### toExcelStruct {#toExcelStruct--}
Indicates whether converting to json struct of the Excel file.
```javascript
toExcelStruct : boolean;
```
**Remarks**
Only for converting range to JSON.
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
### getExportStylePool() {#getExportStylePool--}
```javascript
getExportStylePool() : boolean;
```
### setExportStylePool(boolean) {#setExportStylePool-boolean-}
```javascript
setExportStylePool(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportHyperlinkType() {#getExportHyperlinkType--}
```javascript
getExportHyperlinkType() : JsonExportHyperlinkType;
```
**Returns**
[JsonExportHyperlinkType](../jsonexporthyperlinktype/)
**Remarks**
The default value is [JsonExportHyperlinkType.DisplayString](../jsonexporthyperlinktype.displaystring/);
### setExportHyperlinkType(JsonExportHyperlinkType) {#setExportHyperlinkType-jsonexporthyperlinktype-}
```javascript
setExportHyperlinkType(value: JsonExportHyperlinkType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [JsonExportHyperlinkType](../jsonexporthyperlinktype/) | The value to set. |
**Remarks**
The default value is [JsonExportHyperlinkType.DisplayString](../jsonexporthyperlinktype.displaystring/);
### getSkipEmptyRows() {#getSkipEmptyRows--}
```javascript
getSkipEmptyRows() : boolean;
```
### setSkipEmptyRows(boolean) {#setSkipEmptyRows-boolean-}
```javascript
setSkipEmptyRows(value: boolean) : void;
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
### getSchemas() {#getSchemas--}
```javascript
getSchemas() : string[];
```
**Returns**
string[]
### setSchemas(string[]) {#setSchemas-stringarray-}
```javascript
setSchemas(value: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |
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
### getIndent() {#getIndent--}
```javascript
getIndent() : string;
```
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### setIndent(string) {#setIndent-string-}
```javascript
setIndent(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### getExportNestedStructure() {#getExportNestedStructure--}
```javascript
getExportNestedStructure() : boolean;
```
### setExportNestedStructure(boolean) {#setExportNestedStructure-boolean-}
```javascript
setExportNestedStructure(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportEmptyCells() {#getExportEmptyCells--}
```javascript
getExportEmptyCells() : boolean;
```
### setExportEmptyCells(boolean) {#setExportEmptyCells-boolean-}
```javascript
setExportEmptyCells(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```javascript
getAlwaysExportAsJsonObject() : boolean;
```
### setAlwaysExportAsJsonObject(boolean) {#setAlwaysExportAsJsonObject-boolean-}
```javascript
setAlwaysExportAsJsonObject(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getToExcelStruct() {#getToExcelStruct--}
```javascript
getToExcelStruct() : boolean;
```
**Remarks**
Only for converting range to JSON.
### setToExcelStruct(boolean) {#setToExcelStruct-boolean-}
```javascript
setToExcelStruct(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for converting range to JSON.
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
