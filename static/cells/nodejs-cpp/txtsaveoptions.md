##TxtSaveOptions
Represents the save options for csvtab delimitedother text format.
## TxtSaveOptions class
Represents the save options for csv/tab delimited/other text format.
```javascript
class TxtSaveOptions extends SaveOptions;
```
## Constructors
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getSeparator()](#getSeparator--)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets char Delimiter of text file. |
| [setSeparator(string)](#setSeparator-string-)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets char Delimiter of text file. |
| [getSeparatorString()](#getSeparatorString--)| <b>@deprecated.</b> Please use the 'separatorString' property instead. Gets and sets a string value as separator. |
| [setSeparatorString(string)](#setSeparatorString-string-)| <b>@deprecated.</b> Please use the 'separatorString' property instead. Gets and sets a string value as separator. |
| [getEncoding()](#getEncoding--)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. |
| [getQuoteType()](#getQuoteType--)| <b>@deprecated.</b> Please use the 'quoteType' property instead. Gets or sets how to quote values in the exported text file. |
| [setQuoteType(TxtValueQuoteType)](#setQuoteType-txtvaluequotetype-)| <b>@deprecated.</b> Please use the 'quoteType' property instead. Gets or sets how to quote values in the exported text file. |
| [getFormatStrategy()](#getFormatStrategy--)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string. |
| [setFormatStrategy(CellValueFormatStrategy)](#setFormatStrategy-cellvalueformatstrategy-)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--)| <b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The data provider for saving workbook in light mode. |
| [setLightCellsDataProvider(LightCellsDataProvider)](#setLightCellsDataProvider-lightcellsdataprovider-)| <b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The data provider for saving workbook in light mode. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--)| <b>@deprecated.</b> Please use the 'trimLeadingBlankRowAndColumn' property instead. Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [setTrimLeadingBlankRowAndColumn(boolean)](#setTrimLeadingBlankRowAndColumn-boolean-)| <b>@deprecated.</b> Please use the 'trimLeadingBlankRowAndColumn' property instead. Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--)| <b>@deprecated.</b> Please use the 'trimTailingBlankCells' property instead. Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [setTrimTailingBlankCells(boolean)](#setTrimTailingBlankCells-boolean-)| <b>@deprecated.</b> Please use the 'trimTailingBlankCells' property instead. Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--)| <b>@deprecated.</b> Please use the 'keepSeparatorsForBlankRow' property instead. Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [setKeepSeparatorsForBlankRow(boolean)](#setKeepSeparatorsForBlankRow-boolean-)| <b>@deprecated.</b> Please use the 'keepSeparatorsForBlankRow' property instead. Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [getExportArea()](#getExportArea--)| <b>@deprecated.</b> Please use the 'exportArea' property instead. The range of cells to be exported. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| <b>@deprecated.</b> Please use the 'exportArea' property instead. The range of cells to be exported. |
| [getExportQuotePrefix()](#getExportQuotePrefix--)| <b>@deprecated.</b> Please use the 'exportQuotePrefix' property instead. Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false. |
| [setExportQuotePrefix(boolean)](#setExportQuotePrefix-boolean-)| <b>@deprecated.</b> Please use the 'exportQuotePrefix' property instead. Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.QuotePrefix](../style.quoteprefix/) is true for it. Default is false. |
| [getExportAllSheets()](#getExportAllSheets--)| <b>@deprecated.</b> Please use the 'exportAllSheets' property instead. Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
| [setExportAllSheets(boolean)](#setExportAllSheets-boolean-)| <b>@deprecated.</b> Please use the 'exportAllSheets' property instead. Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
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
### getSeparator() {#getSeparator--}
```javascript
getSeparator() : string;
```
### setSeparator(string) {#setSeparator-string-}
```javascript
setSeparator(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSeparatorString() {#getSeparatorString--}
```javascript
getSeparatorString() : string;
```
### setSeparatorString(string) {#setSeparatorString-string-}
```javascript
setSeparatorString(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getEncoding() {#getEncoding--}
```javascript
getEncoding() : EncodingType;
```
**Returns**
[EncodingType](../encodingtype/)
### setEncoding(EncodingType) {#setEncoding-encodingtype-}
```javascript
setEncoding(value: EncodingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |
### getQuoteType() {#getQuoteType--}
```javascript
getQuoteType() : TxtValueQuoteType;
```
**Returns**
[TxtValueQuoteType](../txtvaluequotetype/)
### setQuoteType(TxtValueQuoteType) {#setQuoteType-txtvaluequotetype-}
```javascript
setQuoteType(value: TxtValueQuoteType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TxtValueQuoteType](../txtvaluequotetype/) | The value to set. |
### getFormatStrategy() {#getFormatStrategy--}
```javascript
getFormatStrategy() : CellValueFormatStrategy;
```
**Returns**
[CellValueFormatStrategy](../cellvalueformatstrategy/)
### setFormatStrategy(CellValueFormatStrategy) {#setFormatStrategy-cellvalueformatstrategy-}
```javascript
setFormatStrategy(value: CellValueFormatStrategy) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueFormatStrategy](../cellvalueformatstrategy/) | The value to set. |
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```javascript
getLightCellsDataProvider() : LightCellsDataProvider;
```
**Returns**
[LightCellsDataProvider](../lightcellsdataprovider/)
### setLightCellsDataProvider(LightCellsDataProvider) {#setLightCellsDataProvider-lightcellsdataprovider-}
```javascript
setLightCellsDataProvider(value: LightCellsDataProvider) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../lightcellsdataprovider/) | The value to set. |
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```javascript
getTrimLeadingBlankRowAndColumn() : boolean;
```
**Remarks**
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../lightcellsdataprovider/) or by speicifing [ExportArea](../exportarea/)
### setTrimLeadingBlankRowAndColumn(boolean) {#setTrimLeadingBlankRowAndColumn-boolean-}
```javascript
setTrimLeadingBlankRowAndColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [LightCellsDataProvider](../lightcellsdataprovider/) or by speicifing [ExportArea](../exportarea/)
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```javascript
getTrimTailingBlankCells() : boolean;
```
**Remarks**
When saving with LightCells mode and the [ExportArea](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [LightCellsDataProvider](../lightcellsdataprovider/)
### setTrimTailingBlankCells(boolean) {#setTrimTailingBlankCells-boolean-}
```javascript
setTrimTailingBlankCells(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
When saving with LightCells mode and the [ExportArea](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [LightCellsDataProvider](../lightcellsdataprovider/)
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```javascript
getKeepSeparatorsForBlankRow() : boolean;
```
### setKeepSeparatorsForBlankRow(boolean) {#setKeepSeparatorsForBlankRow-boolean-}
```javascript
setKeepSeparatorsForBlankRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportArea() {#getExportArea--}
```javascript
getExportArea() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
**Remarks**
If the exported area has been specified, [TrimLeadingBlankRowAndColumn](../trimleadingblankrowandcolumn/) will takes no effect.
### setExportArea(CellArea) {#setExportArea-cellarea-}
```javascript
setExportArea(value: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |
**Remarks**
If the exported area has been specified, [TrimLeadingBlankRowAndColumn](../trimleadingblankrowandcolumn/) will takes no effect.
### getExportQuotePrefix() {#getExportQuotePrefix--}
```javascript
getExportQuotePrefix() : boolean;
```
### setExportQuotePrefix(boolean) {#setExportQuotePrefix-boolean-}
```javascript
setExportQuotePrefix(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportAllSheets() {#getExportAllSheets--}
```javascript
getExportAllSheets() : boolean;
```
**Remarks**
The defult value is false.
### setExportAllSheets(boolean) {#setExportAllSheets-boolean-}
```javascript
setExportAllSheets(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The defult value is false.
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
