##SpreadsheetML2003SaveOptions
Represents the options for saving Excel 2003 spreadml file.
## SpreadsheetML2003SaveOptions class
Represents the options for saving Excel 2003 spreadml file.
```javascript
class SpreadsheetML2003SaveOptions extends SaveOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for saving Excel 2003 spreadml file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isIndentedFormatting](#isIndentedFormatting--)| boolean | Causes child elements to be indented. |
| [limitAsXls](#limitAsXls--)| boolean | Limit as xls, the max row index is 65535 and the max column index is 255. |
| [exportColumnIndexOfCell](#exportColumnIndexOfCell--)| boolean | The default value is false, it means that column index  will be ignored if the cell is contiguous to the previous cell. |
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
Creates the options for saving Excel 2003 spreadml file.
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
### isIndentedFormatting {#isIndentedFormatting--}
Causes child elements to be indented.
```javascript
isIndentedFormatting : boolean;
```
**Remarks**
The default value is true. If the value is false, it will reduce the size of the xml file
### limitAsXls {#limitAsXls--}
Limit as xls, the max row index is 65535 and the max column index is 255.
```javascript
limitAsXls : boolean;
```
### exportColumnIndexOfCell {#exportColumnIndexOfCell--}
The default value is false, it means that column index  will be ignored if the cell is contiguous to the previous cell.
```javascript
exportColumnIndexOfCell : boolean;
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
