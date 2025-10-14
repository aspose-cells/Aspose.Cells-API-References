---
title: TxtLoadOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the options for loading text file.
type: docs
url: /javascript-cpp/txtloadoptions/
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
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| Sets the default print paper size from default printer's setting. |


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


