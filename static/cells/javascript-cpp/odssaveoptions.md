##OdsSaveOptions
Represents the options of saving ods file.
## OdsSaveOptions class
Represents the options of saving ods file.
```javascript
class OdsSaveOptions extends SaveOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options of saving ods file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates the options of saving ods file. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [generatorType](#generatorType--)| OdsGeneratorType | Gets and sets the generator of the ods file. |
| [isStrictSchema11](#isStrictSchema11--)| boolean | Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [odfStrictVersion](#odfStrictVersion--)| OpenDocumentFormatVersionType | Gets and sets the ODF version. |
| [ignorePivotTables](#ignorePivotTables--)| boolean | Indicates whether saving pivot tables. |
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
Creates the options of saving ods file.
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
### constructor(SaveFormat) {#constructor-saveformat-}
Creates the options of saving ods file.
```javascript
constructor(saveFormat: SaveFormat);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be [SaveFormat.Ods](../saveformat.ods/), [SaveFormat.Ots](../saveformat.ots/),         /// [SaveFormat.Fods](../saveformat.fods/) or [SaveFormat.Sxc](../saveformat.sxc/),         /// otherwise the saved format will be set as [SaveFormat.Ods](../saveformat.ods/) automatically. |
### generatorType {#generatorType--}
Gets and sets the generator of the ods file.
```javascript
generatorType : OdsGeneratorType;
```
### isStrictSchema11 {#isStrictSchema11--}
Indicates whether the ods file should be saved as ODF format version 1.1. Default is false.
```javascript
isStrictSchema11 : boolean;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.
### odfStrictVersion {#odfStrictVersion--}
Gets and sets the ODF version.
```javascript
odfStrictVersion : OpenDocumentFormatVersionType;
```
### ignorePivotTables {#ignorePivotTables--}
Indicates whether saving pivot tables.
```javascript
ignorePivotTables : boolean;
```
**Remarks**
The pivot table feature of OpenOffice has fewer settings compared to Excel, so their results of pivot table have many differences. Sometimes it's better to ingore these pivot tables when saving .ods file.
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
