---
title: "TxtLoadOptions"
linktitle: "TxtLoadOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options for loading text file."
type: docs
weight: 4390
url: /nodejs/aspose.cells/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

```js
new TxtLoadOptions()
```

Creates the options for loading text file. The default load file type is CSV .

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(loadFormat)](#constructor-overload1) | Creates the options for loading text file. |
| [getAutoFilter()](#getautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [getAutoFitterOptions()](#getautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getcheckdatavalid) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [getConvertDateTimeData()](#getconvertdatetimedata) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [getConvertNumericData()](#getconvertnumericdata) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getdefaultstylesettings) | Gets the default style settings for initializing styles of the workbook |
| [getEncoding()](#getencoding) | Gets and sets the default encoding. Only applies for csv file. |
| [getExtendToNextSheet()](#getextendtonextsheet) | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is  |
| [getFontConfigs()](#getfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [getHeaderColumnsCount()](#getheadercolumnscount) | The count of header columns to be repeated for extended sheets. The header columns specified by this property will be du |
| [getHeaderRowsCount()](#getheaderrowscount) | The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicat |
| [getIgnoreNotPrinted()](#getignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getIgnoreUselessShapes()](#getignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [getInterruptMonitor()](#getinterruptmonitor) | Gets and sets the interrupt monitor. |
| [getKeepPrecision()](#getkeepprecision) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [getLanguageCode()](#getlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [getLightCellsDataHandler()](#getlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getloadfilter) | The filter to denote how to load data. |
| [getLoadFormat()](#getloadformat) | Gets the load format. The value of the property is LoadFormat integer constant. |
| [getLoadStyleStrategy()](#getloadstylestrategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of |
| [getLocale()](#getlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMaxColumnCount()](#getmaxcolumncount) | The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extende |
| [getMaxRowCount()](#getmaxrowcount) | The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to n |
| [getMemorySetting()](#getmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [getParsingFormulaOnOpen()](#getparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [getParsingPivotCachedRecords()](#getparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [getPassword()](#getpassword) | Gets and set the password of the workbook. |
| [getPreferredParsers()](#getpreferredparsers) | Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column  |
| [getPreservePaddingSpacesInFormula()](#getpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [getRegion()](#getregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [getSeparator()](#getseparator) | Gets and sets character separator of text file. |
| [getSeparatorString()](#getseparatorstring) | Gets and sets a string value as separator. |
| [getStandardFont()](#getstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [getStandardFontSize()](#getstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [getTextQualifier()](#gettextqualifier) | Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier wil |
| [getTreatConsecutiveDelimitersAsOne()](#gettreatconsecutivedelimitersasone) | Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#gettreatquoteprefixasvalue) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it |
| [hasFormula()](#hasformula) | Indicates whether the text is formula if it starts with "=". |
| [hasTextQualifier()](#hastextqualifier) | Whether there is text qualifier for cell value. Default is true. |
| [isMultiEncoded()](#ismultiencoded) | True means that the file contains several encoding. |
| [setAutoFilter()](#setautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [setAutoFitterOptions()](#setautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [setCheckDataValid()](#setcheckdatavalid) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [setConvertDateTimeData()](#setconvertdatetimedata) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertNumericData()](#setconvertnumericdata) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [setEncoding()](#setencoding) | Gets and sets the default encoding. Only applies for csv file. |
| [setExtendToNextSheet()](#setextendtonextsheet) | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is  |
| [setFontConfigs()](#setfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [setHasFormula()](#sethasformula) | Indicates whether the text is formula if it starts with "=". |
| [setHasTextQualifier()](#sethastextqualifier) | Whether there is text qualifier for cell value. Default is true. |
| [setHeaderColumnsCount()](#setheadercolumnscount) | The count of header columns to be repeated for extended sheets. The header columns specified by this property will be du |
| [setHeaderRowsCount()](#setheaderrowscount) | The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicat |
| [setIgnoreNotPrinted()](#setignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [setIgnoreUselessShapes()](#setignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [setInterruptMonitor()](#setinterruptmonitor) | Gets and sets the interrupt monitor. |
| [setKeepPrecision()](#setkeepprecision) | Indicates whether not parsing a string value if the length is 15. |
| [setKeepUnparsedData()](#setkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [setLanguageCode()](#setlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [setLightCellsDataHandler()](#setlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [setLoadFilter()](#setloadfilter) | The filter to denote how to load data. |
| [setLoadStyleStrategy()](#setloadstylestrategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of |
| [setLocale()](#setlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [setMaxColumnCount()](#setmaxcolumncount) | The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extende |
| [setMaxRowCount()](#setmaxrowcount) | The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to n |
| [setMemorySetting()](#setmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [setMultiEncoded()](#setmultiencoded) | True means that the file contains several encoding. |
| [setPaperSize(type)](#setpapersize) | Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will  |
| [setParsingFormulaOnOpen()](#setparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [setParsingPivotCachedRecords()](#setparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [setPassword()](#setpassword) | Gets and set the password of the workbook. |
| [setPreferredParsers()](#setpreferredparsers) | Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column  |
| [setPreservePaddingSpacesInFormula()](#setpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [setRegion()](#setregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [setSeparator()](#setseparator) | Gets and sets character separator of text file. |
| [setSeparatorString()](#setseparatorstring) | Gets and sets a string value as separator. |
| [setStandardFont()](#setstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [setStandardFontSize()](#setstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [setTextQualifier()](#settextqualifier) | Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier wil |
| [setTreatConsecutiveDelimitersAsOne()](#settreatconsecutivedelimitersasone) | Whether consecutive delimiters should be treated as one. |
| [setTreatQuotePrefixAsValue()](#settreatquoteprefixasvalue) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it |

### constructor_overload$1(loadFormat) {#constructor-overload1}

Creates the options for loading text file.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | LoadFormat |

### getAutoFilter() {#getautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### getAutoFitterOptions() {#getautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### getCheckDataValid() {#getcheckdatavalid}

Check whether data is valid in the template file.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### getConvertDateTimeData() {#getconvertdatetimedata}

Gets or sets a value that indicates whether the string in text file is converted to date data.

### getConvertNumericData() {#getconvertnumericdata}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

### getDefaultStyleSettings() {#getdefaultstylesettings}

Gets the default style settings for initializing styles of the workbook

### getEncoding() {#getencoding}

Gets and sets the default encoding. Only applies for csv file.

### getExtendToNextSheet() {#getextendtonextsheet}

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

### getFontConfigs() {#getfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### getHeaderColumnsCount() {#getheadercolumnscount}

The count of header columns to be repeated for extended sheets. The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

### getHeaderRowsCount() {#getheaderrowscount}

The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

### getIgnoreNotPrinted() {#getignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

### getIgnoreUselessShapes() {#getignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### getInterruptMonitor() {#getinterruptmonitor}

Gets and sets the interrupt monitor.

### getKeepPrecision() {#getkeepprecision}

Indicates whether not parsing a string value if the length is 15.

### getKeepUnparsedData() {#getkeepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### getLanguageCode() {#getlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### getLightCellsDataHandler() {#getlightcellsdatahandler}

The data handler for processing cells data when reading template file.

### getLoadFilter() {#getloadfilter}

The filter to denote how to load data.

### getLoadFormat() {#getloadformat}

Gets the load format. The value of the property is LoadFormat integer constant.

### getLoadStyleStrategy() {#getloadstylestrategy}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of the property is TxtLoadStyleStrategy integer constant.

### getLocale() {#getlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### getMaxColumnCount() {#getmaxcolumncount}

The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header columns(HeaderColumnsCount). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### getMaxRowCount() {#getmaxrowcount}

The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header rows(HeaderRowsCount). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### getMemorySetting() {#getmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### getParsingFormulaOnOpen() {#getparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### getParsingPivotCachedRecords() {#getparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### getPassword() {#getpassword}

Gets and set the password of the workbook.

### getPreferredParsers() {#getpreferredparsers}

Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

### getPreservePaddingSpacesInFormula() {#getpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### getRegion() {#getregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### getSeparator() {#getseparator}

Gets and sets character separator of text file.

### getSeparatorString() {#getseparatorstring}

Gets and sets a string value as separator.

### getStandardFont() {#getstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getStandardFontSize() {#getstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getTextQualifier() {#gettextqualifier}

Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier will become true automatically.

### getTreatConsecutiveDelimitersAsOne() {#gettreatconsecutivedelimitersasone}

Whether consecutive delimiters should be treated as one.

### getTreatQuotePrefixAsValue() {#gettreatquoteprefixasvalue}

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and Style.QuotePrefix will be set as true for the cell.

### hasFormula() {#hasformula}

Indicates whether the text is formula if it starts with "=".

### hasTextQualifier() {#hastextqualifier}

Whether there is text qualifier for cell value. Default is true.

### isMultiEncoded() {#ismultiencoded}

True means that the file contains several encoding.

### setAutoFilter() {#setautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### setAutoFitterOptions() {#setautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### setCheckDataValid() {#setcheckdatavalid}

Check whether data is valid in the template file.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### setConvertDateTimeData() {#setconvertdatetimedata}

Gets or sets a value that indicates whether the string in text file is converted to date data.

### setConvertNumericData() {#setconvertnumericdata}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

### setEncoding() {#setencoding}

Gets and sets the default encoding. Only applies for csv file.

### setExtendToNextSheet() {#setextendtonextsheet}

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

### setFontConfigs() {#setfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### setHasFormula() {#sethasformula}

Indicates whether the text is formula if it starts with "=".

### setHasTextQualifier() {#sethastextqualifier}

Whether there is text qualifier for cell value. Default is true.

### setHeaderColumnsCount() {#setheadercolumnscount}

The count of header columns to be repeated for extended sheets. The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

### setHeaderRowsCount() {#setheaderrowscount}

The count of header rows to be repeated for extended sheets. The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when ExtendToNextSheet is true.

### setIgnoreNotPrinted() {#setignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

### setIgnoreUselessShapes() {#setignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### setInterruptMonitor() {#setinterruptmonitor}

Gets and sets the interrupt monitor.

### setKeepPrecision() {#setkeepprecision}

Indicates whether not parsing a string value if the length is 15.

### setKeepUnparsedData() {#setkeepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### setLanguageCode() {#setlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### setLightCellsDataHandler() {#setlightcellsdatahandler}

The data handler for processing cells data when reading template file.

### setLoadFilter() {#setloadfilter}

The filter to denote how to load data.

### setLoadStyleStrategy() {#setloadstylestrategy}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of the property is TxtLoadStyleStrategy integer constant.

### setLocale() {#setlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### setMaxColumnCount() {#setmaxcolumncount}

The maximum count of columns to be imported for one sheet. Those columns exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header columns(HeaderColumnsCount). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### setMaxRowCount() {#setmaxrowcount}

The maximum count of rows to be imported for one sheet. Those rows exceeding this limit will be ignored or extended to next sheet according to ExtendToNextSheet. This count includes the header rows(HeaderRowsCount). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### setMemorySetting() {#setmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### setMultiEncoded() {#setmultiencoded}

True means that the file contains several encoding.

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | PaperSizeType |

### setParsingFormulaOnOpen() {#setparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### setParsingPivotCachedRecords() {#setparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### setPassword() {#setpassword}

Gets and set the password of the workbook.

### setPreferredParsers() {#setpreferredparsers}

Gets and sets preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

### setPreservePaddingSpacesInFormula() {#setpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### setRegion() {#setregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### setSeparator() {#setseparator}

Gets and sets character separator of text file.

### setSeparatorString() {#setseparatorstring}

Gets and sets a string value as separator.

### setStandardFont() {#setstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setStandardFontSize() {#setstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setTextQualifier() {#settextqualifier}

Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, HasTextQualifier will become true automatically.

### setTreatConsecutiveDelimitersAsOne() {#settreatconsecutivedelimitersasone}

Whether consecutive delimiters should be treated as one.

### setTreatQuotePrefixAsValue() {#settreatquoteprefixasvalue}

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and Style.QuotePrefix will be set as true for the cell.
