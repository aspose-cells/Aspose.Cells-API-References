##TxtSaveOptions
Represents the save options for csvtab delimitedother text format.
## TxtSaveOptions class
Represents the save options for csv/tab delimited/other text format.
```javascript
class TxtSaveOptions extends SaveOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates text file save options. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates text file save options. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [separator](#separator--)| string | Gets and sets char Delimiter of text file. |
| [separatorString](#separatorString--)| string | Gets and sets a string value as separator. |
| [encoding](#encoding--)| EncodingType | Gets and sets the default encoding. |
| [quoteType](#quoteType--)| TxtValueQuoteType | Gets or sets how to quote values in the exported text file. |
| [formatStrategy](#formatStrategy--)| CellValueFormatStrategy | Gets and sets the format strategy when exporting the cell value as string. |
| [lightCellsDataProvider](#lightCellsDataProvider--)| LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [trimLeadingBlankRowAndColumn](#trimLeadingBlankRowAndColumn--)| boolean | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [trimTailingBlankCells](#trimTailingBlankCells--)| boolean | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [keepSeparatorsForBlankRow](#keepSeparatorsForBlankRow--)| boolean | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [exportArea](#exportArea--)| CellArea | The range of cells to be exported. |
| [exportQuotePrefix](#exportQuotePrefix--)| boolean | Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false. |
| [exportAllSheets](#exportAllSheets--)| boolean | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
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
Creates text file save options.
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
Creates text file save options.
```javascript
constructor(saveFormat: SaveFormat);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be [SaveFormat.Csv](../saveformat.csv/) or [SaveFormat.Tsv](../saveformat.tsv/),         /// otherwise the saved format will be set as [SaveFormat.Csv](../saveformat.csv/) automatically. |
### separator {#separator--}
Gets and sets char Delimiter of text file.
```javascript
separator : string;
```
### separatorString {#separatorString--}
Gets and sets a string value as separator.
```javascript
separatorString : string;
```
### encoding {#encoding--}
Gets and sets the default encoding.
```javascript
encoding : EncodingType;
```
### quoteType {#quoteType--}
Gets or sets how to quote values in the exported text file.
```javascript
quoteType : TxtValueQuoteType;
```
### formatStrategy {#formatStrategy--}
Gets and sets the format strategy when exporting the cell value as string.
```javascript
formatStrategy : CellValueFormatStrategy;
```
### lightCellsDataProvider {#lightCellsDataProvider--}
The data provider for saving workbook in light mode.
```javascript
lightCellsDataProvider : LightCellsDataProvider;
```
### trimLeadingBlankRowAndColumn {#trimLeadingBlankRowAndColumn--}
Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.
```javascript
trimLeadingBlankRowAndColumn : boolean;
```
**Remarks**
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../lightcellsdataprovider/) or by speicifing [ExportArea](../exportarea/)
### trimTailingBlankCells {#trimTailingBlankCells--}
Indicates whether tailing blank cells in one row should be trimmed. Default is false.
```javascript
trimTailingBlankCells : boolean;
```
**Remarks**
When saving with LightCells mode and the [ExportArea](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [LightCellsDataProvider](../lightcellsdataprovider/)
### keepSeparatorsForBlankRow {#keepSeparatorsForBlankRow--}
Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.
```javascript
keepSeparatorsForBlankRow : boolean;
```
### exportArea {#exportArea--}
The range of cells to be exported.
```javascript
exportArea : CellArea;
```
**Remarks**
If the exported area has been specified, [TrimLeadingBlankRowAndColumn](../trimleadingblankrowandcolumn/) will takes no effect.
### exportQuotePrefix {#exportQuotePrefix--}
Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false.
```javascript
exportQuotePrefix : boolean;
```
### exportAllSheets {#exportAllSheets--}
Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.
```javascript
exportAllSheets : boolean;
```
**Remarks**
The defult value is false.
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
