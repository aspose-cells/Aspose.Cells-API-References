---
title: "TxtLoadOptions Class"
linktitle: "TxtLoadOptions"
articleTitle: "TxtLoadOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options for loading text file."
type: docs
weight: 7150
url: /python-java/asposecells.api/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

## Constructors

| Name | Description |
| --- | --- |
| [TxtLoadOptions](#constructor) | Creates the options for loading text file. The default load file type is CSV . |
| [TxtLoadOptions](#constructor) | Creates the options for loading text file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Separator](#separator) | char | Gets and sets character separator of text file. |
| [SeparatorString](#separatorstring) | String | Gets and sets a string value as separator. |
| [IsMultiEncoded](#ismultiencoded) | boolean | True means that the file contains several encoding. |
| [PreferredParsers](#preferredparsers) | ICustomParser[] | Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column  |
| [HasFormula](#hasformula) | boolean | Indicates whether the text is formula if it starts with "=". |
| [HasTextQualifier](#hastextqualifier) | boolean | Whether there is text qualifier for cell value. Default is true. |
| [TextQualifier](#textqualifier) | char | Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier wil |
| [TreatConsecutiveDelimitersAsOne](#treatconsecutivedelimitersasone) | boolean | Whether consecutive delimiters should be treated as one. |
| [TreatQuotePrefixAsValue](#treatquoteprefixasvalue) | boolean | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it |
| [ExtendToNextSheet](#extendtonextsheet) | boolean | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is  |
| [HeaderRowsCount](#headerrowscount) | int | The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicat |
| [HeaderColumnsCount](#headercolumnscount) | int | The count of header columns to be repeated for extended sheets. The header columns specified by this property will be du |
| [MaxRowCount](#maxrowcount) | int | The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to n |
| [MaxColumnCount](#maxcolumncount) | int | The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extende |
| [Encoding](#encoding) | Encoding | Gets and sets the default encoding. Only applies for csv file. |
| [LoadStyleStrategy](#loadstylestrategy) | int | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of |
| [ConvertNumericData](#convertnumericdata) | boolean | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [ConvertDateTimeData](#convertdatetimedata) | boolean | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [KeepPrecision](#keepprecision) | boolean | Indicates whether not parsing a string value if the length is 15. |
| [LoadFormat](#loadformat) | int | Gets the load format. The value of the property is LoadFormat integer constant. |
| [Password](#password) | String | Gets and set the password of the workbook. |
| [ParsingFormulaOnOpen](#parsingformulaonopen) | boolean | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [ParsingPivotCachedRecords](#parsingpivotcachedrecords) | boolean | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [LanguageCode](#languagecode) | int | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [Region](#region) | int | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [Locale](#locale) | Locale | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [DefaultStyleSettings](#defaultstylesettings) | DefaultStyleSettings | Gets the default style settings for initializing styles of the workbook |
| [StandardFont](#standardfont) | String | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [StandardFontSize](#standardfontsize) | float | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [InterruptMonitor](#interruptmonitor) | AbstractInterruptMonitor | Gets and sets the interrupt monitor. |
| [IgnoreNotPrinted](#ignorenotprinted) | boolean | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [CheckDataValid](#checkdatavalid) | boolean | Check whether data is valid in the template file. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [KeepUnparsedData](#keepunparseddata) | boolean | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [LoadFilter](#loadfilter) | LoadFilter | The filter to denote how to load data. |
| [LightCellsDataHandler](#lightcellsdatahandler) | LightCellsDataHandler | The data handler for processing cells data when reading template file. |
| [MemorySetting](#memorysetting) | int | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [AutoFitterOptions](#autofitteroptions) | AutoFitterOptions | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [AutoFilter](#autofilter) | boolean | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [FontConfigs](#fontconfigs) | IndividualFontConfigs | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [IgnoreUselessShapes](#ignoreuselessshapes) | boolean | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [PreservePaddingSpacesInFormula](#preservepaddingspacesinformula) | boolean | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |

## Methods

| Name | Description |
| --- | --- |
| [setPaperSize](#setpapersize) | Sets the default print paper size from default printer's setting.

If there is no setting about paper size,MS Excel will |

### TxtLoadOptions() (1 of 2) {#constructor}

Creates the options for loading text file. The default load file type is CSV .

---

### TxtLoadOptions(loadFormat) (2 of 2) {#constructor-1}

Creates the options for loading text file.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | A LoadFormat value. The loading format |

### TxtLoadOptions.Separator property {#separator}

Gets and sets character separator of text file.

**Type:** char

### TxtLoadOptions.SeparatorString property {#separatorstring}

Gets and sets a string value as separator.

**Type:** String

### TxtLoadOptions.IsMultiEncoded property {#ismultiencoded}

True means that the file contains several encoding.

**Type:** boolean

### TxtLoadOptions.PreferredParsers property {#preferredparsers}

Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

**Type:** ICustomParser[]

### TxtLoadOptions.HasFormula property {#hasformula}

Indicates whether the text is formula if it starts with "=".

**Type:** boolean

### TxtLoadOptions.HasTextQualifier property {#hastextqualifier}

Whether there is text qualifier for cell value. Default is true.

**Type:** boolean

### TxtLoadOptions.TextQualifier property {#textqualifier}

Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier will become true automatically.

**Type:** char

### TxtLoadOptions.TreatConsecutiveDelimitersAsOne property {#treatconsecutivedelimitersasone}

Whether consecutive delimiters should be treated as one.

**Type:** boolean

### TxtLoadOptions.TreatQuotePrefixAsValue property {#treatquoteprefixasvalue}

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and Style.QuotePrefix will be set as true for the cell.

**Type:** boolean

### TxtLoadOptions.ExtendToNextSheet property {#extendtonextsheet}

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

**Type:** boolean

### TxtLoadOptions.HeaderRowsCount property {#headerrowscount}

The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

**Type:** int

### TxtLoadOptions.HeaderColumnsCount property {#headercolumnscount}

The count of header columns to be repeated for extended sheets. The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

**Type:** int

### TxtLoadOptions.MaxRowCount property {#maxrowcount}

The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet . This count includes the header rows( HeaderRowsCount ). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Type:** int

### TxtLoadOptions.MaxColumnCount property {#maxcolumncount}

The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet . This count includes the header columns( HeaderColumnsCount ). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Type:** int

### TxtLoadOptions.Encoding property {#encoding}

Gets and sets the default encoding. Only applies for csv file.

**Type:** Encoding

### TxtLoadOptions.LoadStyleStrategy property {#loadstylestrategy}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of the property is TxtLoadStyleStrategy integer constant.

**Type:** int

### TxtLoadOptions.ConvertNumericData property {#convertnumericdata}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

**Type:** boolean

### TxtLoadOptions.ConvertDateTimeData property {#convertdatetimedata}

Gets or sets a value that indicates whether the string in text file is converted to date data.

**Type:** boolean

### TxtLoadOptions.KeepPrecision property {#keepprecision}

Indicates whether not parsing a string value if the length is 15.

**Type:** boolean

### TxtLoadOptions.LoadFormat property {#loadformat}

Gets the load format. The value of the property is LoadFormat integer constant.

**Type:** int

### TxtLoadOptions.Password property {#password}

Gets and set the password of the workbook.

**Type:** String

### TxtLoadOptions.ParsingFormulaOnOpen property {#parsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Type:** boolean

### TxtLoadOptions.ParsingPivotCachedRecords property {#parsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Type:** boolean

### TxtLoadOptions.LanguageCode property {#languagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

**Type:** int

### TxtLoadOptions.Region property {#region}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant. If you do not want to use the region saved in the file, please reset it after reading the file.

**Type:** int

### TxtLoadOptions.Locale property {#locale}

Gets and sets the Locale used for workbook at the time the file was loaded.

**Type:** Locale

### TxtLoadOptions.DefaultStyleSettings property {#defaultstylesettings}

Gets the default style settings for initializing styles of the workbook

**Type:** DefaultStyleSettings

### TxtLoadOptions.StandardFont property {#standardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** String

### TxtLoadOptions.StandardFontSize property {#standardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** float

### TxtLoadOptions.InterruptMonitor property {#interruptmonitor}

Gets and sets the interrupt monitor.

**Type:** AbstractInterruptMonitor

### TxtLoadOptions.IgnoreNotPrinted property {#ignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

**Type:** boolean

### TxtLoadOptions.CheckDataValid property {#checkdatavalid}

Check whether data is valid in the template file.

**Type:** boolean

### TxtLoadOptions.CheckExcelRestriction property {#checkexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Type:** boolean

### TxtLoadOptions.KeepUnparsedData property {#keepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Type:** boolean

### TxtLoadOptions.LoadFilter property {#loadfilter}

The filter to denote how to load data.

**Type:** LoadFilter

### TxtLoadOptions.LightCellsDataHandler property {#lightcellsdatahandler}

The data handler for processing cells data when reading template file.

**Type:** LightCellsDataHandler

### TxtLoadOptions.MemorySetting property {#memorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

**Type:** int

### TxtLoadOptions.AutoFitterOptions property {#autofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

**Type:** AutoFitterOptions

### TxtLoadOptions.AutoFilter property {#autofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Type:** boolean

### TxtLoadOptions.FontConfigs property {#fontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

**Type:** IndividualFontConfigs

### TxtLoadOptions.IgnoreUselessShapes property {#ignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

**Type:** boolean

### TxtLoadOptions.PreservePaddingSpacesInFormula property {#preservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

**Type:** boolean

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting.

If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A PaperSizeType value. The default paper size. |
