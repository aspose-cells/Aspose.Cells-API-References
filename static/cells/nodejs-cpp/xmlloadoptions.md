##XmlLoadOptions
Represents the options of loading xml.
## XmlLoadOptions class
Represents the options of loading xml.
```javascript
class XmlLoadOptions extends LoadOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Represents the options of loading xml file. |
| [constructor(LoadOptions)](#constructor-loadoptions-)| Constructs from a parent object convertible to this. |
| [constructor(LoadFormat)](#constructor-loadformat-)| Represents the options of loading xml file. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [startCell](#startCell--)| string | Gets and sets the start cell. |
| [isXmlMap](#isXmlMap--)| boolean | Indicates whether mapping xml to Excel. The default value is false. |
| [containsMultipleWorksheets](#containsMultipleWorksheets--)| boolean | Indicates whether importing xml as multiple worksheets. |
| [convertNumericOrDate](#convertNumericOrDate--)| boolean | Indicates whether converting the value in xml file to numeric or date. |
| [numberFormat](#numberFormat--)| string | Gets and sets the format of numeric value. |
| [dateFormat](#dateFormat--)| string | Gets and sets the format of date value. |
| [ignoreRootAttributes](#ignoreRootAttributes--)| boolean | Indicates whether ignore attributes of the root element. |
| [loadFormat](#loadFormat--)| LoadFormat | Readonly. Gets the load format. |
| [password](#password--)| string | Gets and set the password of the workbook. |
| [parsingFormulaOnOpen](#parsingFormulaOnOpen--)| boolean | Indicates whether parsing the formula when reading the file. |
| [parsingPivotCachedRecords](#parsingPivotCachedRecords--)| boolean | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [languageCode](#languageCode--)| CountryCode | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](#region--)| CountryCode | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [defaultStyleSettings](#defaultStyleSettings--)| DefaultStyleSettings | Readonly. Gets the default style settings for initializing styles of the workbook |
| [interruptMonitor](#interruptMonitor--)| AbstractInterruptMonitor | Gets and sets the interrupt monitor. |
| [ignoreNotPrinted](#ignoreNotPrinted--)| boolean | Ignore the data which are not printed if directly printing the file |
| [checkDataValid](#checkDataValid--)| boolean | Check whether data is valid in the template file. |
| [checkExcelRestriction](#checkExcelRestriction--)| boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [keepUnparsedData](#keepUnparsedData--)| boolean | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [loadFilter](#loadFilter--)| LoadFilter | The filter to denote how to load data. |
| [lightCellsDataHandler](#lightCellsDataHandler--)| LightCellsDataHandler | The data handler for processing cells data when reading template file. |
| [memorySetting](#memorySetting--)| MemorySetting | Gets or sets the memory mode for loaded workbook. |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [autoFitterOptions](#autoFitterOptions--)| AutoFitterOptions | Gets and sets the auto fitter options |
| [autoFilter](#autoFilter--)| boolean | Indicates whether auto filtering the data when loading the files. |
| [fontConfigs](#fontConfigs--)| IndividualFontConfigs | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [ignoreUselessShapes](#ignoreUselessShapes--)| boolean | Indicates whether ignoring useless shapes. |
| [preservePaddingSpacesInFormula](#preservePaddingSpacesInFormula--)| boolean | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
## Methods
| Method | Description |
| --- | --- |
| [getStartCell()](#getStartCell--)| <b>@deprecated.</b> Please use the 'startCell' property instead. Gets and sets the start cell. |
| [setStartCell(string)](#setStartCell-string-)| <b>@deprecated.</b> Please use the 'startCell' property instead. Gets and sets the start cell. |
| [isXmlMap()](#isXmlMap--)| <b>@deprecated.</b> Please use the 'isXmlMap' property instead. Indicates whether mapping xml to Excel. The default value is false. |
| [setIsXmlMap(boolean)](#setIsXmlMap-boolean-)| <b>@deprecated.</b> Please use the 'isXmlMap' property instead. Indicates whether mapping xml to Excel. The default value is false. |
| [getContainsMultipleWorksheets()](#getContainsMultipleWorksheets--)| <b>@deprecated.</b> Please use the 'containsMultipleWorksheets' property instead. Indicates whether importing xml as multiple worksheets. |
| [setContainsMultipleWorksheets(boolean)](#setContainsMultipleWorksheets-boolean-)| <b>@deprecated.</b> Please use the 'containsMultipleWorksheets' property instead. Indicates whether importing xml as multiple worksheets. |
| [getConvertNumericOrDate()](#getConvertNumericOrDate--)| <b>@deprecated.</b> Please use the 'convertNumericOrDate' property instead. Indicates whether converting the value in xml file to numeric or date. |
| [setConvertNumericOrDate(boolean)](#setConvertNumericOrDate-boolean-)| <b>@deprecated.</b> Please use the 'convertNumericOrDate' property instead. Indicates whether converting the value in xml file to numeric or date. |
| [get_NumberFormat()](#get_NumberFormat--)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Gets and sets the format of numeric value. |
| [setNumberFormat(string)](#setNumberFormat-string-)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Gets and sets the format of numeric value. |
| [get_DateFormat()](#get_DateFormat--)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets and sets the format of date value. |
| [setDateFormat(string)](#setDateFormat-string-)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets and sets the format of date value. |
| [getIgnoreRootAttributes()](#getIgnoreRootAttributes--)| <b>@deprecated.</b> Please use the 'ignoreRootAttributes' property instead. Indicates whether ignore attributes of the root element. |
| [setIgnoreRootAttributes(boolean)](#setIgnoreRootAttributes-boolean-)| <b>@deprecated.</b> Please use the 'ignoreRootAttributes' property instead. Indicates whether ignore attributes of the root element. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getLoadFormat()](#getLoadFormat--)| <b>@deprecated.</b> Please use the 'loadFormat' property instead. Gets the load format. |
| [getPassword()](#getPassword--)| <b>@deprecated.</b> Please use the 'password' property instead. Gets and set the password of the workbook. |
| [setPassword(string)](#setPassword-string-)| <b>@deprecated.</b> Please use the 'password' property instead. Gets and set the password of the workbook. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--)| <b>@deprecated.</b> Please use the 'parsingFormulaOnOpen' property instead. Indicates whether parsing the formula when reading the file. |
| [setParsingFormulaOnOpen(boolean)](#setParsingFormulaOnOpen-boolean-)| <b>@deprecated.</b> Please use the 'parsingFormulaOnOpen' property instead. Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--)| <b>@deprecated.</b> Please use the 'parsingPivotCachedRecords' property instead. Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [setParsingPivotCachedRecords(boolean)](#setParsingPivotCachedRecords-boolean-)| <b>@deprecated.</b> Please use the 'parsingPivotCachedRecords' property instead. Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [getLanguageCode()](#getLanguageCode--)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getRegion()](#getRegion--)| <b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings used for the Workbook that will be loaded. |
| [setRegion(CountryCode)](#setRegion-countrycode-)| <b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings used for the Workbook that will be loaded. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--)| <b>@deprecated.</b> Please use the 'defaultStyleSettings' property instead. Gets the default style settings for initializing styles of the workbook |
| [getInterruptMonitor()](#getInterruptMonitor--)| <b>@deprecated.</b> Please use the 'interruptMonitor' property instead. Gets and sets the interrupt monitor. |
| [setInterruptMonitor(AbstractInterruptMonitor)](#setInterruptMonitor-abstractinterruptmonitor-)| <b>@deprecated.</b> Please use the 'interruptMonitor' property instead. Gets and sets the interrupt monitor. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--)| <b>@deprecated.</b> Please use the 'ignoreNotPrinted' property instead. Ignore the data which are not printed if directly printing the file |
| [setIgnoreNotPrinted(boolean)](#setIgnoreNotPrinted-boolean-)| <b>@deprecated.</b> Please use the 'ignoreNotPrinted' property instead. Ignore the data which are not printed if directly printing the file |
| [getCheckDataValid()](#getCheckDataValid--)| <b>@deprecated.</b> Please use the 'checkDataValid' property instead. Check whether data is valid in the template file. |
| [setCheckDataValid(boolean)](#setCheckDataValid-boolean-)| <b>@deprecated.</b> Please use the 'checkDataValid' property instead. Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [getKeepUnparsedData()](#getKeepUnparsedData--)| <b>@deprecated.</b> Please use the 'keepUnparsedData' property instead. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [setKeepUnparsedData(boolean)](#setKeepUnparsedData-boolean-)| <b>@deprecated.</b> Please use the 'keepUnparsedData' property instead. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [getLoadFilter()](#getLoadFilter--)| <b>@deprecated.</b> Please use the 'loadFilter' property instead. The filter to denote how to load data. |
| [setLoadFilter(LoadFilter)](#setLoadFilter-loadfilter-)| <b>@deprecated.</b> Please use the 'loadFilter' property instead. The filter to denote how to load data. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--)| <b>@deprecated.</b> Please use the 'lightCellsDataHandler' property instead. The data handler for processing cells data when reading template file. |
| [setLightCellsDataHandler(LightCellsDataHandler)](#setLightCellsDataHandler-lightcellsdatahandler-)| <b>@deprecated.</b> Please use the 'lightCellsDataHandler' property instead. The data handler for processing cells data when reading template file. |
| [getMemorySetting()](#getMemorySetting--)| <b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory mode for loaded workbook. |
| [setMemorySetting(MemorySetting)](#setMemorySetting-memorysetting-)| <b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory mode for loaded workbook. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getAutoFitterOptions()](#getAutoFitterOptions--)| <b>@deprecated.</b> Please use the 'autoFitterOptions' property instead. Gets and sets the auto fitter options |
| [setAutoFitterOptions(AutoFitterOptions)](#setAutoFitterOptions-autofitteroptions-)| <b>@deprecated.</b> Please use the 'autoFitterOptions' property instead. Gets and sets the auto fitter options |
| [getAutoFilter()](#getAutoFilter--)| <b>@deprecated.</b> Please use the 'autoFilter' property instead. Indicates whether auto filtering the data when loading the files. |
| [setAutoFilter(boolean)](#setAutoFilter-boolean-)| <b>@deprecated.</b> Please use the 'autoFilter' property instead. Indicates whether auto filtering the data when loading the files. |
| [getFontConfigs()](#getFontConfigs--)| <b>@deprecated.</b> Please use the 'fontConfigs' property instead. Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [setFontConfigs(IndividualFontConfigs)](#setFontConfigs-individualfontconfigs-)| <b>@deprecated.</b> Please use the 'fontConfigs' property instead. Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--)| <b>@deprecated.</b> Please use the 'ignoreUselessShapes' property instead. Indicates whether ignoring useless shapes. |
| [setIgnoreUselessShapes(boolean)](#setIgnoreUselessShapes-boolean-)| <b>@deprecated.</b> Please use the 'ignoreUselessShapes' property instead. Indicates whether ignoring useless shapes. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--)| <b>@deprecated.</b> Please use the 'preservePaddingSpacesInFormula' property instead. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [setPreservePaddingSpacesInFormula(boolean)](#setPreservePaddingSpacesInFormula-boolean-)| <b>@deprecated.</b> Please use the 'preservePaddingSpacesInFormula' property instead. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| Sets the default print paper size from default printer's setting. |
### constructor() {#constructor--}
Represents the options of loading xml file.
```javascript
constructor();
```
### constructor(LoadOptions) {#constructor-loadoptions-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: LoadOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | LoadOptions | The parent object. |
### constructor(LoadFormat) {#constructor-loadformat-}
Represents the options of loading xml file.
```javascript
constructor(type: LoadFormat);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [LoadFormat](../loadformat/) | The load format type. |
### startCell {#startCell--}
Gets and sets the start cell.
```javascript
startCell : string;
```
**Remarks**
Only works when the file is not speadsheetML or mapping xml to Excel.
### isXmlMap {#isXmlMap--}
Indicates whether mapping xml to Excel. The default value is false.
```javascript
isXmlMap : boolean;
```
### containsMultipleWorksheets {#containsMultipleWorksheets--}
Indicates whether importing xml as multiple worksheets.
```javascript
containsMultipleWorksheets : boolean;
```
### convertNumericOrDate {#convertNumericOrDate--}
Indicates whether converting the value in xml file to numeric or date.
```javascript
convertNumericOrDate : boolean;
```
### numberFormat {#numberFormat--}
Gets and sets the format of numeric value.
```javascript
numberFormat : string;
```
### dateFormat {#dateFormat--}
Gets and sets the format of date value.
```javascript
dateFormat : string;
```
### ignoreRootAttributes {#ignoreRootAttributes--}
Indicates whether ignore attributes of the root element.
```javascript
ignoreRootAttributes : boolean;
```
### loadFormat {#loadFormat--}
Readonly. Gets the load format.
```javascript
loadFormat : LoadFormat;
```
### password {#password--}
Gets and set the password of the workbook.
```javascript
password : string;
```
### parsingFormulaOnOpen {#parsingFormulaOnOpen--}
Indicates whether parsing the formula when reading the file.
```javascript
parsingFormulaOnOpen : boolean;
```
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
### parsingPivotCachedRecords {#parsingPivotCachedRecords--}
Indicates whether parsing pivot cached records when loading the file. The default value is false.
```javascript
parsingPivotCachedRecords : boolean;
```
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
### languageCode {#languageCode--}
Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.
```javascript
languageCode : CountryCode;
```
### region {#region--}
Gets or sets the regional settings used for the Workbook that will be loaded.
```javascript
region : CountryCode;
```
**Remarks**
The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [WorkbookSettings.Region](../workbooksettings.region/) of the workbook will use the same region with this property.
### defaultStyleSettings {#defaultStyleSettings--}
Readonly. Gets the default style settings for initializing styles of the workbook
```javascript
defaultStyleSettings : DefaultStyleSettings;
```
### interruptMonitor {#interruptMonitor--}
Gets and sets the interrupt monitor.
```javascript
interruptMonitor : AbstractInterruptMonitor;
```
### ignoreNotPrinted {#ignoreNotPrinted--}
Ignore the data which are not printed if directly printing the file
```javascript
ignoreNotPrinted : boolean;
```
**Remarks**
Only for xlsx file.
### checkDataValid {#checkDataValid--}
Check whether data is valid in the template file.
```javascript
checkDataValid : boolean;
```
### checkExcelRestriction {#checkExcelRestriction--}
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.
```javascript
checkExcelRestriction : boolean;
```
### keepUnparsedData {#keepUnparsedData--}
Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.
```javascript
keepUnparsedData : boolean;
```
**Remarks**
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
### loadFilter {#loadFilter--}
The filter to denote how to load data.
```javascript
loadFilter : LoadFilter;
```
### lightCellsDataHandler {#lightCellsDataHandler--}
The data handler for processing cells data when reading template file.
```javascript
lightCellsDataHandler : LightCellsDataHandler;
```
### memorySetting {#memorySetting--}
Gets or sets the memory mode for loaded workbook.
```javascript
memorySetting : MemorySetting;
```
**Remarks**
For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).
### warningCallback {#warningCallback--}
Gets or sets warning callback.
```javascript
warningCallback : IWarningCallback;
```
### autoFitterOptions {#autoFitterOptions--}
Gets and sets the auto fitter options
```javascript
autoFitterOptions : AutoFitterOptions;
```
**Remarks**
Only for xlsx ,spreadsheetML file now.
### autoFilter {#autoFilter--}
Indicates whether auto filtering the data when loading the files.
```javascript
autoFilter : boolean;
```
**Remarks**
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
### fontConfigs {#fontConfigs--}
Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load.
```javascript
fontConfigs : IndividualFontConfigs;
```
### ignoreUselessShapes {#ignoreUselessShapes--}
Indicates whether ignoring useless shapes.
```javascript
ignoreUselessShapes : boolean;
```
**Remarks**
Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.
### preservePaddingSpacesInFormula {#preservePaddingSpacesInFormula--}
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
```javascript
preservePaddingSpacesInFormula : boolean;
```
**Remarks**
After loading workbook from template file with this option, [FormulaSettings.PreservePaddingSpaces](../formulasettings.preservepaddingspaces/) will be set to the same value with this property.
### getStartCell() {#getStartCell--}
```javascript
getStartCell() : string;
```
**Remarks**
Only works when the file is not speadsheetML or mapping xml to Excel.
### setStartCell(string) {#setStartCell-string-}
```javascript
setStartCell(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Only works when the file is not speadsheetML or mapping xml to Excel.
### isXmlMap() {#isXmlMap--}
```javascript
isXmlMap() : boolean;
```
### setIsXmlMap(boolean) {#setIsXmlMap-boolean-}
```javascript
setIsXmlMap(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getContainsMultipleWorksheets() {#getContainsMultipleWorksheets--}
```javascript
getContainsMultipleWorksheets() : boolean;
```
### setContainsMultipleWorksheets(boolean) {#setContainsMultipleWorksheets-boolean-}
```javascript
setContainsMultipleWorksheets(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getConvertNumericOrDate() {#getConvertNumericOrDate--}
```javascript
getConvertNumericOrDate() : boolean;
```
### setConvertNumericOrDate(boolean) {#setConvertNumericOrDate-boolean-}
```javascript
setConvertNumericOrDate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### get_NumberFormat() {#get_NumberFormat--}
```javascript
get_NumberFormat() : string;
```
### setNumberFormat(string) {#setNumberFormat-string-}
```javascript
setNumberFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### get_DateFormat() {#get_DateFormat--}
```javascript
get_DateFormat() : string;
```
### setDateFormat(string) {#setDateFormat-string-}
```javascript
setDateFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getIgnoreRootAttributes() {#getIgnoreRootAttributes--}
```javascript
getIgnoreRootAttributes() : boolean;
```
### setIgnoreRootAttributes(boolean) {#setIgnoreRootAttributes-boolean-}
```javascript
setIgnoreRootAttributes(value: boolean) : void;
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
### getLoadFormat() {#getLoadFormat--}
```javascript
getLoadFormat() : LoadFormat;
```
**Returns**
[LoadFormat](../loadformat/)
### getPassword() {#getPassword--}
```javascript
getPassword() : string;
```
### setPassword(string) {#setPassword-string-}
```javascript
setPassword(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```javascript
getParsingFormulaOnOpen() : boolean;
```
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
### setParsingFormulaOnOpen(boolean) {#setParsingFormulaOnOpen-boolean-}
```javascript
setParsingFormulaOnOpen(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```javascript
getParsingPivotCachedRecords() : boolean;
```
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
### setParsingPivotCachedRecords(boolean) {#setParsingPivotCachedRecords-boolean-}
```javascript
setParsingPivotCachedRecords(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
### getLanguageCode() {#getLanguageCode--}
```javascript
getLanguageCode() : CountryCode;
```
**Returns**
[CountryCode](../countrycode/)
### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}
```javascript
setLanguageCode(value: CountryCode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |
### getRegion() {#getRegion--}
```javascript
getRegion() : CountryCode;
```
**Returns**
[CountryCode](../countrycode/)
**Remarks**
The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [WorkbookSettings.Region](../workbooksettings.region/) of the workbook will use the same region with this property.
### setRegion(CountryCode) {#setRegion-countrycode-}
```javascript
setRegion(value: CountryCode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |
**Remarks**
The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [WorkbookSettings.Region](../workbooksettings.region/) of the workbook will use the same region with this property.
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```javascript
getDefaultStyleSettings() : DefaultStyleSettings;
```
**Returns**
[DefaultStyleSettings](../defaultstylesettings/)
### getInterruptMonitor() {#getInterruptMonitor--}
```javascript
getInterruptMonitor() : AbstractInterruptMonitor;
```
**Returns**
[AbstractInterruptMonitor](../abstractinterruptmonitor/)
### setInterruptMonitor(AbstractInterruptMonitor) {#setInterruptMonitor-abstractinterruptmonitor-}
```javascript
setInterruptMonitor(value: AbstractInterruptMonitor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../abstractinterruptmonitor/) | The value to set. |
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```javascript
getIgnoreNotPrinted() : boolean;
```
**Remarks**
Only for xlsx file.
### setIgnoreNotPrinted(boolean) {#setIgnoreNotPrinted-boolean-}
```javascript
setIgnoreNotPrinted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for xlsx file.
### getCheckDataValid() {#getCheckDataValid--}
```javascript
getCheckDataValid() : boolean;
```
### setCheckDataValid(boolean) {#setCheckDataValid-boolean-}
```javascript
setCheckDataValid(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
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
### getKeepUnparsedData() {#getKeepUnparsedData--}
```javascript
getKeepUnparsedData() : boolean;
```
**Remarks**
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
### setKeepUnparsedData(boolean) {#setKeepUnparsedData-boolean-}
```javascript
setKeepUnparsedData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
### getLoadFilter() {#getLoadFilter--}
```javascript
getLoadFilter() : LoadFilter;
```
**Returns**
[LoadFilter](../loadfilter/)
### setLoadFilter(LoadFilter) {#setLoadFilter-loadfilter-}
```javascript
setLoadFilter(value: LoadFilter) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../loadfilter/) | The value to set. |
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```javascript
getLightCellsDataHandler() : LightCellsDataHandler;
```
**Returns**
[LightCellsDataHandler](../lightcellsdatahandler/)
### setLightCellsDataHandler(LightCellsDataHandler) {#setLightCellsDataHandler-lightcellsdatahandler-}
```javascript
setLightCellsDataHandler(value: LightCellsDataHandler) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../lightcellsdatahandler/) | The value to set. |
### getMemorySetting() {#getMemorySetting--}
```javascript
getMemorySetting() : MemorySetting;
```
**Returns**
[MemorySetting](../memorysetting/)
**Remarks**
For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).
### setMemorySetting(MemorySetting) {#setMemorySetting-memorysetting-}
```javascript
setMemorySetting(value: MemorySetting) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MemorySetting](../memorysetting/) | The value to set. |
**Remarks**
For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).
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
### getAutoFitterOptions() {#getAutoFitterOptions--}
```javascript
getAutoFitterOptions() : AutoFitterOptions;
```
**Returns**
[AutoFitterOptions](../autofitteroptions/)
**Remarks**
Only for xlsx ,spreadsheetML file now.
### setAutoFitterOptions(AutoFitterOptions) {#setAutoFitterOptions-autofitteroptions-}
```javascript
setAutoFitterOptions(value: AutoFitterOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitterOptions](../autofitteroptions/) | The value to set. |
**Remarks**
Only for xlsx ,spreadsheetML file now.
### getAutoFilter() {#getAutoFilter--}
```javascript
getAutoFilter() : boolean;
```
**Remarks**
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
### setAutoFilter(boolean) {#setAutoFilter-boolean-}
```javascript
setAutoFilter(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
### getFontConfigs() {#getFontConfigs--}
```javascript
getFontConfigs() : IndividualFontConfigs;
```
**Returns**
[IndividualFontConfigs](../individualfontconfigs/)
### setFontConfigs(IndividualFontConfigs) {#setFontConfigs-individualfontconfigs-}
```javascript
setFontConfigs(value: IndividualFontConfigs) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../individualfontconfigs/) | The value to set. |
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```javascript
getIgnoreUselessShapes() : boolean;
```
**Remarks**
Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.
### setIgnoreUselessShapes(boolean) {#setIgnoreUselessShapes-boolean-}
```javascript
setIgnoreUselessShapes(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```javascript
getPreservePaddingSpacesInFormula() : boolean;
```
**Remarks**
After loading workbook from template file with this option, [FormulaSettings.PreservePaddingSpaces](../formulasettings.preservepaddingspaces/) will be set to the same value with this property.
### setPreservePaddingSpacesInFormula(boolean) {#setPreservePaddingSpacesInFormula-boolean-}
```javascript
setPreservePaddingSpacesInFormula(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
After loading workbook from template file with this option, [FormulaSettings.PreservePaddingSpaces](../formulasettings.preservepaddingspaces/) will be set to the same value with this property.
### setPaperSize(PaperSizeType) {#setPaperSize-papersizetype-}
Sets the default print paper size from default printer's setting.
```javascript
setPaperSize(type: PaperSizeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PaperSizeType](../papersizetype/) | The default paper size. |
**Remarks**
If there is no setting about paper size,MS Excel will use default printer's setting.
