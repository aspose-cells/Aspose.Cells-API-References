##JsonSaveOptions
Represents the options of saving the workbook as a json file.
## JsonSaveOptions class
Represents the options of saving the workbook as a json file.
```javascript
class JsonSaveOptions extends SaveOptions;
```
## Constructors
| Name | Description |
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
