##TxtLoadOptions
Represents the options for loading text file.
## TxtLoadOptions class
Represents the options for loading text file.
```javascript
class TxtLoadOptions extends AbstractTextLoadOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for loading text file. |
| [constructor(AbstractTextLoadOptions)](#constructor-abstracttextloadoptions-)| Constructs from a parent object convertible to this. |
| [constructor(LoadFormat)](#constructor-loadformat-)| Creates the options for loading text file. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [separator](#separator--)| string | Gets and sets character separator of text file. |
| [separatorString](#separatorString--)| string | Gets and sets a string value as separator. |
| [isMultiEncoded](#isMultiEncoded--)| boolean | True means that the file contains several encoding. |
| [hasFormula](#hasFormula--)| boolean | Indicates whether the text is formula if it starts with "=". |
| [hasTextQualifier](#hasTextQualifier--)| boolean | Whether there is text qualifier for cell value. Default is true. |
| [textQualifier](#textQualifier--)| string | Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [treatConsecutiveDelimitersAsOne](#treatConsecutiveDelimitersAsOne--)| boolean | Whether consecutive delimiters should be treated as one. |
| [treatQuotePrefixAsValue](#treatQuotePrefixAsValue--)| boolean | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell. |
| [extendToNextSheet](#extendToNextSheet--)| boolean | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [headerRowsCount](#headerRowsCount--)| number | The count of header rows to be repeated for extended sheets. |
| [headerColumnsCount](#headerColumnsCount--)| number | The count of header columns to be repeated for extended sheets. |
| [maxRowCount](#maxRowCount--)| number | The maximum count of rows to be imported for one sheet. |
| [maxColumnCount](#maxColumnCount--)| number | The maximum count of columns to be imported for one sheet. |
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
| [encoding](#encoding--)| EncodingType | Gets and sets the default encoding. Only applies for csv file. |
| [loadStyleStrategy](#loadStyleStrategy--)| TxtLoadStyleStrategy | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [convertNumericData](#convertNumericData--)| boolean | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [convertDateTimeData](#convertDateTimeData--)| boolean | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [keepPrecision](#keepPrecision--)| boolean | Indicates whether not parsing a string value if the length is 15. |
## Methods
| Method | Description |
| --- | --- |
| [getSeparator()](#getSeparator--)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets character separator of text file. |
| [setSeparator(string)](#setSeparator-string-)| <b>@deprecated.</b> Please use the 'separator' property instead. Gets and sets character separator of text file. |
| [getSeparatorString()](#getSeparatorString--)| <b>@deprecated.</b> Please use the 'separatorString' property instead. Gets and sets a string value as separator. |
| [setSeparatorString(string)](#setSeparatorString-string-)| <b>@deprecated.</b> Please use the 'separatorString' property instead. Gets and sets a string value as separator. |
| [isMultiEncoded()](#isMultiEncoded--)| <b>@deprecated.</b> Please use the 'isMultiEncoded' property instead. True means that the file contains several encoding. |
| [setIsMultiEncoded(boolean)](#setIsMultiEncoded-boolean-)| <b>@deprecated.</b> Please use the 'isMultiEncoded' property instead. True means that the file contains several encoding. |
| [getHasFormula()](#getHasFormula--)| <b>@deprecated.</b> Please use the 'hasFormula' property instead. Indicates whether the text is formula if it starts with "=". |
| [setHasFormula(boolean)](#setHasFormula-boolean-)| <b>@deprecated.</b> Please use the 'hasFormula' property instead. Indicates whether the text is formula if it starts with "=". |
| [getHasTextQualifier()](#getHasTextQualifier--)| <b>@deprecated.</b> Please use the 'hasTextQualifier' property instead. Whether there is text qualifier for cell value. Default is true. |
| [setHasTextQualifier(boolean)](#setHasTextQualifier-boolean-)| <b>@deprecated.</b> Please use the 'hasTextQualifier' property instead. Whether there is text qualifier for cell value. Default is true. |
| [getTextQualifier()](#getTextQualifier--)| <b>@deprecated.</b> Please use the 'textQualifier' property instead. Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [setTextQualifier(string)](#setTextQualifier-string-)| <b>@deprecated.</b> Please use the 'textQualifier' property instead. Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--)| <b>@deprecated.</b> Please use the 'treatConsecutiveDelimitersAsOne' property instead. Whether consecutive delimiters should be treated as one. |
| [setTreatConsecutiveDelimitersAsOne(boolean)](#setTreatConsecutiveDelimitersAsOne-boolean-)| <b>@deprecated.</b> Please use the 'treatConsecutiveDelimitersAsOne' property instead. Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--)| <b>@deprecated.</b> Please use the 'treatQuotePrefixAsValue' property instead. Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell. |
| [setTreatQuotePrefixAsValue(boolean)](#setTreatQuotePrefixAsValue-boolean-)| <b>@deprecated.</b> Please use the 'treatQuotePrefixAsValue' property instead. Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell. |
| [getExtendToNextSheet()](#getExtendToNextSheet--)| <b>@deprecated.</b> Please use the 'extendToNextSheet' property instead. Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [setExtendToNextSheet(boolean)](#setExtendToNextSheet-boolean-)| <b>@deprecated.</b> Please use the 'extendToNextSheet' property instead. Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [getHeaderRowsCount()](#getHeaderRowsCount--)| <b>@deprecated.</b> Please use the 'headerRowsCount' property instead. The count of header rows to be repeated for extended sheets. |
| [setHeaderRowsCount(number)](#setHeaderRowsCount-number-)| <b>@deprecated.</b> Please use the 'headerRowsCount' property instead. The count of header rows to be repeated for extended sheets. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--)| <b>@deprecated.</b> Please use the 'headerColumnsCount' property instead. The count of header columns to be repeated for extended sheets. |
| [setHeaderColumnsCount(number)](#setHeaderColumnsCount-number-)| <b>@deprecated.</b> Please use the 'headerColumnsCount' property instead. The count of header columns to be repeated for extended sheets. |
| [getMaxRowCount()](#getMaxRowCount--)| <b>@deprecated.</b> Please use the 'maxRowCount' property instead. The maximum count of rows to be imported for one sheet. |
| [setMaxRowCount(number)](#setMaxRowCount-number-)| <b>@deprecated.</b> Please use the 'maxRowCount' property instead. The maximum count of rows to be imported for one sheet. |
| [getMaxColumnCount()](#getMaxColumnCount--)| <b>@deprecated.</b> Please use the 'maxColumnCount' property instead. The maximum count of columns to be imported for one sheet. |
| [setMaxColumnCount(number)](#setMaxColumnCount-number-)| <b>@deprecated.</b> Please use the 'maxColumnCount' property instead. The maximum count of columns to be imported for one sheet. |
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
| [getEncoding()](#getEncoding--)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. Only applies for csv file. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. Only applies for csv file. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--)| <b>@deprecated.</b> Please use the 'loadStyleStrategy' property instead. Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [setLoadStyleStrategy(TxtLoadStyleStrategy)](#setLoadStyleStrategy-txtloadstylestrategy-)| <b>@deprecated.</b> Please use the 'loadStyleStrategy' property instead. Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getConvertNumericData()](#getConvertNumericData--)| <b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [setConvertNumericData(boolean)](#setConvertNumericData-boolean-)| <b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [getConvertDateTimeData()](#getConvertDateTimeData--)| <b>@deprecated.</b> Please use the 'convertDateTimeData' property instead. Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [setConvertDateTimeData(boolean)](#setConvertDateTimeData-boolean-)| <b>@deprecated.</b> Please use the 'convertDateTimeData' property instead. Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [getKeepPrecision()](#getKeepPrecision--)| <b>@deprecated.</b> Please use the 'keepPrecision' property instead. Indicates whether not parsing a string value if the length is 15. |
| [setKeepPrecision(boolean)](#setKeepPrecision-boolean-)| <b>@deprecated.</b> Please use the 'keepPrecision' property instead. Indicates whether not parsing a string value if the length is 15. |
### constructor() {#constructor--}
Creates the options for loading text file.
```javascript
constructor();
```
**Remarks**
The default load file type is CSV .
### constructor(AbstractTextLoadOptions) {#constructor-abstracttextloadoptions-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: AbstractTextLoadOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | AbstractTextLoadOptions | The parent object. |
### constructor(LoadFormat) {#constructor-loadformat-}
Creates the options for loading text file.
```javascript
constructor(loadFormat: LoadFormat);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | [LoadFormat](../loadformat/) | The loading format |
### separator {#separator--}
Gets and sets character separator of text file.
```javascript
separator : string;
```
### separatorString {#separatorString--}
Gets and sets a string value as separator.
```javascript
separatorString : string;
```
### isMultiEncoded {#isMultiEncoded--}
True means that the file contains several encoding.
```javascript
isMultiEncoded : boolean;
```
### hasFormula {#hasFormula--}
Indicates whether the text is formula if it starts with "=".
```javascript
hasFormula : boolean;
```
### hasTextQualifier {#hasTextQualifier--}
Whether there is text qualifier for cell value. Default is true.
```javascript
hasTextQualifier : boolean;
```
### textQualifier {#textQualifier--}
Specifies the text qualifier for cell values. Default qualifier is '"'.
```javascript
textQualifier : string;
```
**Remarks**
When setting this property, [HasTextQualifier](../hastextqualifier/) will become true automatically.
### treatConsecutiveDelimitersAsOne {#treatConsecutiveDelimitersAsOne--}
Whether consecutive delimiters should be treated as one.
```javascript
treatConsecutiveDelimitersAsOne : boolean;
```
### treatQuotePrefixAsValue {#treatQuotePrefixAsValue--}
Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell.
```javascript
treatQuotePrefixAsValue : boolean;
```
### extendToNextSheet {#extendToNextSheet--}
Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.
```javascript
extendToNextSheet : boolean;
```
**Remarks**
If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.
### headerRowsCount {#headerRowsCount--}
The count of header rows to be repeated for extended sheets.
```javascript
headerRowsCount : number;
```
**Remarks**
The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### headerColumnsCount {#headerColumnsCount--}
The count of header columns to be repeated for extended sheets.
```javascript
headerColumnsCount : number;
```
**Remarks**
The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### maxRowCount {#maxRowCount--}
The maximum count of rows to be imported for one sheet.
```javascript
maxRowCount : number;
```
**Remarks**
Those rows exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header rows([HeaderRowsCount](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### maxColumnCount {#maxColumnCount--}
The maximum count of columns to be imported for one sheet.
```javascript
maxColumnCount : number;
```
**Remarks**
Those columns exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header columns([HeaderColumnsCount](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
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
### encoding {#encoding--}
Gets and sets the default encoding. Only applies for csv file.
```javascript
encoding : EncodingType;
```
### loadStyleStrategy {#loadStyleStrategy--}
Indicates the strategy to apply style for parsed values when converting string value to number or datetime.
```javascript
loadStyleStrategy : TxtLoadStyleStrategy;
```
### convertNumericData {#convertNumericData--}
Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.
```javascript
convertNumericData : boolean;
```
### convertDateTimeData {#convertDateTimeData--}
Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true.
```javascript
convertDateTimeData : boolean;
```
### keepPrecision {#keepPrecision--}
Indicates whether not parsing a string value if the length is 15.
```javascript
keepPrecision : boolean;
```
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
### isMultiEncoded() {#isMultiEncoded--}
```javascript
isMultiEncoded() : boolean;
```
### setIsMultiEncoded(boolean) {#setIsMultiEncoded-boolean-}
```javascript
setIsMultiEncoded(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHasFormula() {#getHasFormula--}
```javascript
getHasFormula() : boolean;
```
### setHasFormula(boolean) {#setHasFormula-boolean-}
```javascript
setHasFormula(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHasTextQualifier() {#getHasTextQualifier--}
```javascript
getHasTextQualifier() : boolean;
```
### setHasTextQualifier(boolean) {#setHasTextQualifier-boolean-}
```javascript
setHasTextQualifier(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTextQualifier() {#getTextQualifier--}
```javascript
getTextQualifier() : string;
```
**Remarks**
When setting this property, [HasTextQualifier](../hastextqualifier/) will become true automatically.
### setTextQualifier(string) {#setTextQualifier-string-}
```javascript
setTextQualifier(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
When setting this property, [HasTextQualifier](../hastextqualifier/) will become true automatically.
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```javascript
getTreatConsecutiveDelimitersAsOne() : boolean;
```
### setTreatConsecutiveDelimitersAsOne(boolean) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```javascript
setTreatConsecutiveDelimitersAsOne(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```javascript
getTreatQuotePrefixAsValue() : boolean;
```
### setTreatQuotePrefixAsValue(boolean) {#setTreatQuotePrefixAsValue-boolean-}
```javascript
setTreatQuotePrefixAsValue(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExtendToNextSheet() {#getExtendToNextSheet--}
```javascript
getExtendToNextSheet() : boolean;
```
**Remarks**
If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.
### setExtendToNextSheet(boolean) {#setExtendToNextSheet-boolean-}
```javascript
setExtendToNextSheet(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.
### getHeaderRowsCount() {#getHeaderRowsCount--}
```javascript
getHeaderRowsCount() : number;
```
**Remarks**
The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### setHeaderRowsCount(number) {#setHeaderRowsCount-number-}
```javascript
setHeaderRowsCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```javascript
getHeaderColumnsCount() : number;
```
**Remarks**
The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### setHeaderColumnsCount(number) {#setHeaderColumnsCount-number-}
```javascript
setHeaderColumnsCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.
### getMaxRowCount() {#getMaxRowCount--}
```javascript
getMaxRowCount() : number;
```
**Remarks**
Those rows exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header rows([HeaderRowsCount](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### setMaxRowCount(number) {#setMaxRowCount-number-}
```javascript
setMaxRowCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Those rows exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header rows([HeaderRowsCount](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### getMaxColumnCount() {#getMaxColumnCount--}
```javascript
getMaxColumnCount() : number;
```
**Remarks**
Those columns exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header columns([HeaderColumnsCount](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### setMaxColumnCount(number) {#setMaxColumnCount-number-}
```javascript
setMaxColumnCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Those columns exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header columns([HeaderColumnsCount](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
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
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```javascript
getLoadStyleStrategy() : TxtLoadStyleStrategy;
```
**Returns**
[TxtLoadStyleStrategy](../txtloadstylestrategy/)
### setLoadStyleStrategy(TxtLoadStyleStrategy) {#setLoadStyleStrategy-txtloadstylestrategy-}
```javascript
setLoadStyleStrategy(value: TxtLoadStyleStrategy) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TxtLoadStyleStrategy](../txtloadstylestrategy/) | The value to set. |
### getConvertNumericData() {#getConvertNumericData--}
```javascript
getConvertNumericData() : boolean;
```
### setConvertNumericData(boolean) {#setConvertNumericData-boolean-}
```javascript
setConvertNumericData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getConvertDateTimeData() {#getConvertDateTimeData--}
```javascript
getConvertDateTimeData() : boolean;
```
### setConvertDateTimeData(boolean) {#setConvertDateTimeData-boolean-}
```javascript
setConvertDateTimeData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getKeepPrecision() {#getKeepPrecision--}
```javascript
getKeepPrecision() : boolean;
```
### setKeepPrecision(boolean) {#setKeepPrecision-boolean-}
```javascript
setKeepPrecision(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
