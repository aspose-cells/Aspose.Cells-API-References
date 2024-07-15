---
title: TxtLoadOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for loading text file.
type: docs
url: /nodejs-cpp/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

```javascript
class TxtLoadOptions extends AbstractTextLoadOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for loading text file. |
| [constructor(AbstractTextLoadOptions)](#constructor-abstracttextloadoptions-)| Constructs from a parent object convertible to this. |
| [constructor(LoadFormat)](#constructor-loadformat-)| Creates the options for loading text file. |

## Methods

| Method | Description |
| --- | --- |
| [getSeparator()](#getSeparator--)| Gets and sets character separator of text file. |
| [setSeparator(string)](#setSeparator-string-)| Gets and sets character separator of text file. |
| [getSeparatorString()](#getSeparatorString--)| Gets and sets a string value as separator. |
| [setSeparatorString(string)](#setSeparatorString-string-)| Gets and sets a string value as separator. |
| [isMultiEncoded()](#isMultiEncoded--)| True means that the file contains several encoding. |
| [setIsMultiEncoded(boolean)](#setIsMultiEncoded-boolean-)| True means that the file contains several encoding. |
| [getHasFormula()](#getHasFormula--)| Indicates whether the text is formula if it starts with "=". |
| [setHasFormula(boolean)](#setHasFormula-boolean-)| Indicates whether the text is formula if it starts with "=". |
| [getHasTextQualifier()](#getHasTextQualifier--)| Whether there is text qualifier for cell value. Default is true. |
| [setHasTextQualifier(boolean)](#setHasTextQualifier-boolean-)| Whether there is text qualifier for cell value. Default is true. |
| [getTextQualifier()](#getTextQualifier--)| Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [setTextQualifier(string)](#setTextQualifier-string-)| Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--)| Whether consecutive delimiters should be treated as one. |
| [setTreatConsecutiveDelimitersAsOne(boolean)](#setTreatConsecutiveDelimitersAsOne-boolean-)| Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--)| Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell. |
| [setTreatQuotePrefixAsValue(boolean)](#setTreatQuotePrefixAsValue-boolean-)| Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell. |
| [getExtendToNextSheet()](#getExtendToNextSheet--)| Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [setExtendToNextSheet(boolean)](#setExtendToNextSheet-boolean-)| Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [getHeaderRowsCount()](#getHeaderRowsCount--)| The count of header rows to be repeated for extended sheets. |
| [setHeaderRowsCount(number)](#setHeaderRowsCount-number-)| The count of header rows to be repeated for extended sheets. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--)| The count of header columns to be repeated for extended sheets. |
| [setHeaderColumnsCount(number)](#setHeaderColumnsCount-number-)| The count of header columns to be repeated for extended sheets. |
| [getMaxRowCount()](#getMaxRowCount--)| The maximum count of rows to be imported for one sheet. |
| [setMaxRowCount(number)](#setMaxRowCount-number-)| The maximum count of rows to be imported for one sheet. |
| [getMaxColumnCount()](#getMaxColumnCount--)| The maximum count of columns to be imported for one sheet. |
| [setMaxColumnCount(number)](#setMaxColumnCount-number-)| The maximum count of columns to be imported for one sheet. |
| [getLoadFormat()](#getLoadFormat--)| Gets the load format. |
| [getPassword()](#getPassword--)| Gets and set the password of the workbook. |
| [setPassword(string)](#setPassword-string-)| Gets and set the password of the workbook. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--)| Indicates whether parsing the formula when reading the file. |
| [setParsingFormulaOnOpen(boolean)](#setParsingFormulaOnOpen-boolean-)| Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--)| Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [setParsingPivotCachedRecords(boolean)](#setParsingPivotCachedRecords-boolean-)| Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [getLanguageCode()](#getLanguageCode--)| Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getRegion()](#getRegion--)| Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [setRegion(CountryCode)](#setRegion-countrycode-)| Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--)| Gets the default style settings for initializing styles of the workbook |
| [getInterruptMonitor()](#getInterruptMonitor--)| Gets and sets the interrupt monitor. |
| [setInterruptMonitor(AbstractInterruptMonitor)](#setInterruptMonitor-abstractinterruptmonitor-)| Gets and sets the interrupt monitor. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--)| Ignore the data which are not printed if directly printing the file |
| [setIgnoreNotPrinted(boolean)](#setIgnoreNotPrinted-boolean-)| Ignore the data which are not printed if directly printing the file |
| [getCheckDataValid()](#getCheckDataValid--)| Check whether data is valid in the template file. |
| [setCheckDataValid(boolean)](#setCheckDataValid-boolean-)| Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [getKeepUnparsedData()](#getKeepUnparsedData--)| Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [setKeepUnparsedData(boolean)](#setKeepUnparsedData-boolean-)| Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [getLoadFilter()](#getLoadFilter--)| The filter to denote how to load data. |
| [setLoadFilter(LoadFilter)](#setLoadFilter-loadfilter-)| The filter to denote how to load data. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--)| The data handler for processing cells data when reading template file. |
| [setLightCellsDataHandler(LightCellsDataHandler)](#setLightCellsDataHandler-lightcellsdatahandler-)| The data handler for processing cells data when reading template file. |
| [getMemorySetting()](#getMemorySetting--)| Gets or sets the memory usage options. |
| [setMemorySetting(MemorySetting)](#setMemorySetting-memorysetting-)| Gets or sets the memory usage options. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getAutoFitterOptions()](#getAutoFitterOptions--)| Gets and sets the auto fitter options |
| [setAutoFitterOptions(AutoFitterOptions)](#setAutoFitterOptions-autofitteroptions-)| Gets and sets the auto fitter options |
| [getAutoFilter()](#getAutoFilter--)| Indicates whether auto filtering the data when loading the files. |
| [setAutoFilter(boolean)](#setAutoFilter-boolean-)| Indicates whether auto filtering the data when loading the files. |
| [getFontConfigs()](#getFontConfigs--)| Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [Workbook](../workbook/) to load. |
| [setFontConfigs(IndividualFontConfigs)](#setFontConfigs-individualfontconfigs-)| Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [Workbook](../workbook/) to load. |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--)| Indicates whether ignoring useless shapes. |
| [setIgnoreUselessShapes(boolean)](#setIgnoreUselessShapes-boolean-)| Indicates whether ignoring useless shapes. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--)| Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [setPreservePaddingSpacesInFormula(boolean)](#setPreservePaddingSpacesInFormula-boolean-)| Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| Sets the default print paper size from default printer's setting. |
| [getEncoding()](#getEncoding--)| Gets and sets the default encoding. Only applies for csv file. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| Gets and sets the default encoding. Only applies for csv file. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--)| Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [setLoadStyleStrategy(TxtLoadStyleStrategy)](#setLoadStyleStrategy-txtloadstylestrategy-)| Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getConvertNumericData()](#getConvertNumericData--)| Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [setConvertNumericData(boolean)](#setConvertNumericData-boolean-)| Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [getConvertDateTimeData()](#getConvertDateTimeData--)| Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertDateTimeData(boolean)](#setConvertDateTimeData-boolean-)| Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [getKeepPrecision()](#getKeepPrecision--)| Indicates whether not parsing a string value if the length is 15. |
| [setKeepPrecision(boolean)](#setKeepPrecision-boolean-)| Indicates whether not parsing a string value if the length is 15. |


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

### getSeparator() {#getSeparator--}

Gets and sets character separator of text file.

```javascript
getSeparator() : string;
```


### setSeparator(string) {#setSeparator-string-}

Gets and sets character separator of text file.

```javascript
setSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSeparatorString() {#getSeparatorString--}

Gets and sets a string value as separator.

```javascript
getSeparatorString() : string;
```


### setSeparatorString(string) {#setSeparatorString-string-}

Gets and sets a string value as separator.

```javascript
setSeparatorString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isMultiEncoded() {#isMultiEncoded--}

True means that the file contains several encoding.

```javascript
isMultiEncoded() : boolean;
```


### setIsMultiEncoded(boolean) {#setIsMultiEncoded-boolean-}

True means that the file contains several encoding.

```javascript
setIsMultiEncoded(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasFormula() {#getHasFormula--}

Indicates whether the text is formula if it starts with "=".

```javascript
getHasFormula() : boolean;
```


### setHasFormula(boolean) {#setHasFormula-boolean-}

Indicates whether the text is formula if it starts with "=".

```javascript
setHasFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasTextQualifier() {#getHasTextQualifier--}

Whether there is text qualifier for cell value. Default is true.

```javascript
getHasTextQualifier() : boolean;
```


### setHasTextQualifier(boolean) {#setHasTextQualifier-boolean-}

Whether there is text qualifier for cell value. Default is true.

```javascript
setHasTextQualifier(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextQualifier() {#getTextQualifier--}

Specifies the text qualifier for cell values. Default qualifier is '"'.

```javascript
getTextQualifier() : string;
```


**Remarks**

When setting this property, [HasTextQualifier](../hastextqualifier/) will become true automatically.

### setTextQualifier(string) {#setTextQualifier-string-}

Specifies the text qualifier for cell values. Default qualifier is '"'.

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

Whether consecutive delimiters should be treated as one.

```javascript
getTreatConsecutiveDelimitersAsOne() : boolean;
```


### setTreatConsecutiveDelimitersAsOne(boolean) {#setTreatConsecutiveDelimitersAsOne-boolean-}

Whether consecutive delimiters should be treated as one.

```javascript
setTreatConsecutiveDelimitersAsOne(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell.

```javascript
getTreatQuotePrefixAsValue() : boolean;
```


### setTreatQuotePrefixAsValue(boolean) {#setTreatQuotePrefixAsValue-boolean-}

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.QuotePrefix](../style.quoteprefix/) will be set as true for the cell.

```javascript
setTreatQuotePrefixAsValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExtendToNextSheet() {#getExtendToNextSheet--}

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

```javascript
getExtendToNextSheet() : boolean;
```


**Remarks**

If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

### setExtendToNextSheet(boolean) {#setExtendToNextSheet-boolean-}

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

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

The count of header rows to be repeated for extended sheets.

```javascript
getHeaderRowsCount() : number;
```


**Remarks**

The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.

### setHeaderRowsCount(number) {#setHeaderRowsCount-number-}

The count of header rows to be repeated for extended sheets.

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

The count of header columns to be repeated for extended sheets.

```javascript
getHeaderColumnsCount() : number;
```


**Remarks**

The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [ExtendToNextSheet](../extendtonextsheet/) is true.

### setHeaderColumnsCount(number) {#setHeaderColumnsCount-number-}

The count of header columns to be repeated for extended sheets.

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

The maximum count of rows to be imported for one sheet.

```javascript
getMaxRowCount() : number;
```


**Remarks**

Those rows exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header rows([HeaderRowsCount](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### setMaxRowCount(number) {#setMaxRowCount-number-}

The maximum count of rows to be imported for one sheet.

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

The maximum count of columns to be imported for one sheet.

```javascript
getMaxColumnCount() : number;
```


**Remarks**

Those columns exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header columns([HeaderColumnsCount](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### setMaxColumnCount(number) {#setMaxColumnCount-number-}

The maximum count of columns to be imported for one sheet.

```javascript
setMaxColumnCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Those columns exceeding this limit will be ignored or extended to next sheet according to [ExtendToNextSheet](../extendtonextsheet/). This count includes the header columns([HeaderColumnsCount](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### getLoadFormat() {#getLoadFormat--}

Gets the load format.

```javascript
getLoadFormat() : LoadFormat;
```


**Returns**

[LoadFormat](../loadformat/)

### getPassword() {#getPassword--}

Gets and set the password of the workbook.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

Gets and set the password of the workbook.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}

Indicates whether parsing the formula when reading the file.

```javascript
getParsingFormulaOnOpen() : boolean;
```


**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### setParsingFormulaOnOpen(boolean) {#setParsingFormulaOnOpen-boolean-}

Indicates whether parsing the formula when reading the file.

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

Indicates whether parsing pivot cached records when loading the file. The default value is false.

```javascript
getParsingPivotCachedRecords() : boolean;
```


**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### setParsingPivotCachedRecords(boolean) {#setParsingPivotCachedRecords-boolean-}

Indicates whether parsing pivot cached records when loading the file. The default value is false.

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

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
getLanguageCode() : CountryCode;
```


**Returns**

[CountryCode](../countrycode/)

### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
setLanguageCode(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |

### getRegion() {#getRegion--}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded.

```javascript
getRegion() : CountryCode;
```


**Returns**

[CountryCode](../countrycode/)

**Remarks**

If you do not want to use the region  saved in the file, please reset it after reading the file.

### setRegion(CountryCode) {#setRegion-countrycode-}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded.

```javascript
setRegion(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |

**Remarks**

If you do not want to use the region  saved in the file, please reset it after reading the file.

### getDefaultStyleSettings() {#getDefaultStyleSettings--}

Gets the default style settings for initializing styles of the workbook

```javascript
getDefaultStyleSettings() : DefaultStyleSettings;
```


**Returns**

[DefaultStyleSettings](../defaultstylesettings/)

### getInterruptMonitor() {#getInterruptMonitor--}

Gets and sets the interrupt monitor.

```javascript
getInterruptMonitor() : AbstractInterruptMonitor;
```


**Returns**

[AbstractInterruptMonitor](../abstractinterruptmonitor/)

### setInterruptMonitor(AbstractInterruptMonitor) {#setInterruptMonitor-abstractinterruptmonitor-}

Gets and sets the interrupt monitor.

```javascript
setInterruptMonitor(value: AbstractInterruptMonitor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../abstractinterruptmonitor/) | The value to set. |

### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}

Ignore the data which are not printed if directly printing the file

```javascript
getIgnoreNotPrinted() : boolean;
```


**Remarks**

Only for xlsx file.

### setIgnoreNotPrinted(boolean) {#setIgnoreNotPrinted-boolean-}

Ignore the data which are not printed if directly printing the file

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

Check whether data is valid in the template file.

```javascript
getCheckDataValid() : boolean;
```


### setCheckDataValid(boolean) {#setCheckDataValid-boolean-}

Check whether data is valid in the template file.

```javascript
setCheckDataValid(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getKeepUnparsedData() {#getKeepUnparsedData--}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

```javascript
getKeepUnparsedData() : boolean;
```


**Remarks**

For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### setKeepUnparsedData(boolean) {#setKeepUnparsedData-boolean-}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

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

The filter to denote how to load data.

```javascript
getLoadFilter() : LoadFilter;
```


**Returns**

[LoadFilter](../loadfilter/)

### setLoadFilter(LoadFilter) {#setLoadFilter-loadfilter-}

The filter to denote how to load data.

```javascript
setLoadFilter(value: LoadFilter) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../loadfilter/) | The value to set. |

### getLightCellsDataHandler() {#getLightCellsDataHandler--}

The data handler for processing cells data when reading template file.

```javascript
getLightCellsDataHandler() : LightCellsDataHandler;
```


**Returns**

[LightCellsDataHandler](../lightcellsdatahandler/)

### setLightCellsDataHandler(LightCellsDataHandler) {#setLightCellsDataHandler-lightcellsdatahandler-}

The data handler for processing cells data when reading template file.

```javascript
setLightCellsDataHandler(value: LightCellsDataHandler) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../lightcellsdatahandler/) | The value to set. |

### getMemorySetting() {#getMemorySetting--}

Gets or sets the memory usage options.

```javascript
getMemorySetting() : MemorySetting;
```


**Returns**

[MemorySetting](../memorysetting/)

### setMemorySetting(MemorySetting) {#setMemorySetting-memorysetting-}

Gets or sets the memory usage options.

```javascript
setMemorySetting(value: MemorySetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MemorySetting](../memorysetting/) | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getAutoFitterOptions() {#getAutoFitterOptions--}

Gets and sets the auto fitter options

```javascript
getAutoFitterOptions() : AutoFitterOptions;
```


**Returns**

[AutoFitterOptions](../autofitteroptions/)

**Remarks**

Only for xlsx ,spreadsheetML file now.

### setAutoFitterOptions(AutoFitterOptions) {#setAutoFitterOptions-autofitteroptions-}

Gets and sets the auto fitter options

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

Indicates whether auto filtering the data when loading the files.

```javascript
getAutoFilter() : boolean;
```


**Remarks**

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### setAutoFilter(boolean) {#setAutoFilter-boolean-}

Indicates whether auto filtering the data when loading the files.

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

Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [Workbook](../workbook/) to load.

```javascript
getFontConfigs() : IndividualFontConfigs;
```


**Returns**

[IndividualFontConfigs](../individualfontconfigs/)

### setFontConfigs(IndividualFontConfigs) {#setFontConfigs-individualfontconfigs-}

Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [Workbook](../workbook/) to load.

```javascript
setFontConfigs(value: IndividualFontConfigs) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../individualfontconfigs/) | The value to set. |

### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}

Indicates whether ignoring useless shapes.

```javascript
getIgnoreUselessShapes() : boolean;
```


**Remarks**

Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### setIgnoreUselessShapes(boolean) {#setIgnoreUselessShapes-boolean-}

Indicates whether ignoring useless shapes.

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

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```javascript
getPreservePaddingSpacesInFormula() : boolean;
```


**Remarks**

After loading workbook from template file with this option, [FormulaSettings.PreservePaddingSpaces](../formulasettings.preservepaddingspaces/) will be set to the same value with this property.

### setPreservePaddingSpacesInFormula(boolean) {#setPreservePaddingSpacesInFormula-boolean-}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

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

Gets and sets the default encoding. Only applies for csv file.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

Gets and sets the default encoding. Only applies for csv file.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getLoadStyleStrategy() {#getLoadStyleStrategy--}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

```javascript
getLoadStyleStrategy() : TxtLoadStyleStrategy;
```


**Returns**

[TxtLoadStyleStrategy](../txtloadstylestrategy/)

### setLoadStyleStrategy(TxtLoadStyleStrategy) {#setLoadStyleStrategy-txtloadstylestrategy-}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

```javascript
setLoadStyleStrategy(value: TxtLoadStyleStrategy) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TxtLoadStyleStrategy](../txtloadstylestrategy/) | The value to set. |

### getConvertNumericData() {#getConvertNumericData--}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

```javascript
getConvertNumericData() : boolean;
```


### setConvertNumericData(boolean) {#setConvertNumericData-boolean-}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

```javascript
setConvertNumericData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getConvertDateTimeData() {#getConvertDateTimeData--}

Gets or sets a value that indicates whether the string in text file is converted to date data.

```javascript
getConvertDateTimeData() : boolean;
```


### setConvertDateTimeData(boolean) {#setConvertDateTimeData-boolean-}

Gets or sets a value that indicates whether the string in text file is converted to date data.

```javascript
setConvertDateTimeData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getKeepPrecision() {#getKeepPrecision--}

Indicates whether not parsing a string value if the length is 15.

```javascript
getKeepPrecision() : boolean;
```


### setKeepPrecision(boolean) {#setKeepPrecision-boolean-}

Indicates whether not parsing a string value if the length is 15.

```javascript
setKeepPrecision(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


