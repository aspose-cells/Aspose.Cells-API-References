---
title: "HtmlLoadOptions"
linktitle: "HtmlLoadOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents options when importing a html file."
type: docs
weight: 1800
url: /nodejs/aspose.cells/htmlloadoptions/
---

## HtmlLoadOptions class

Represents options when importing a html file.

```js
new HtmlLoadOptions()
```

Creates an options of loading the file.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(loadFormat)](#constructor-overload1) | Creates an options of loading the file. |
| [getAttachedFilesDirectory()](#getattachedfilesdirectory) | The directory that the attached files will be saved to. NOTE: This member is now obsolete. Instead, please use HtmlLoadO |
| [getAutoFilter()](#getautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [getAutoFitColsAndRows()](#getautofitcolsandrows) | Indicates whether auto-fit columns and rows. The default value is false. |
| [getAutoFitterOptions()](#getautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getcheckdatavalid) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [getConvertDateTimeData()](#getconvertdatetimedata) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [getConvertFormulasData()](#getconvertformulasdata) | if true, convert string to formula when string value starts with character '=',the default value is false. NOTE: This pr |
| [getConvertNumericData()](#getconvertnumericdata) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getdefaultstylesettings) | Gets the default style settings for initializing styles of the workbook |
| [getDeleteRedundantSpaces()](#getdeleteredundantspaces) | Indicates whether delete redundant spaces when the text wraps lines using tag. The default value is false. |
| [getDetectLaTeX()](#getdetectlatex) |  |
| [getEncoding()](#getencoding) | Gets and sets the default encoding. Only applies for csv file. |
| [getFontConfigs()](#getfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [getHyperlinkLoadMode()](#gethyperlinkloadmode) | The value of the property is HyperlinkLoadMode integer constant. |
| [getIgnoreNotPrinted()](#getignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getIgnoreUselessShapes()](#getignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [getInterruptMonitor()](#getinterruptmonitor) | Gets and sets the interrupt monitor. |
| [getKeepPrecision()](#getkeepprecision) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [getLanguageCode()](#getlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [getLightCellsDataHandler()](#getlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getloadfilter) | The filter to denote how to load data. |
| [getLoadFormat()](#getloadformat) | Gets the load format. The value of the property is LoadFormat integer constant. |
| [getLoadFormulas()](#getloadformulas) | Indicates whether importing formulas if the original html file contains formulas |
| [getLoadStyleStrategy()](#getloadstylestrategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of |
| [getLocale()](#getlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](#getmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [getParagrahLayoutMode()](#getparagrahlayoutmode) | The value of the property is HtmlParagraphLayoutMode integer constant. |
| [getParsingFormulaOnOpen()](#getparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [getParsingPivotCachedRecords()](#getparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [getPassword()](#getpassword) | Gets and set the password of the workbook. |
| [getPreservePaddingSpacesInFormula()](#getpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [getProgId()](#getprogid) | Gets the program id of creating the file. Only for MHT files. |
| [getRegion()](#getregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [getStandardFont()](#getstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [getStandardFontSize()](#getstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [getSupportDivTag()](#getsupportdivtag) | Indicates whether support the layout of tag when the html file contains it. The default value is false. |
| [getTableLoadOptions()](#gettableloadoptions) | Get the HtmlTableLoadOptionCollection instance |
| [getWarningCallback()](#getwarningcallback) | Gets or sets warning callback. |
| [hasFormula()](#hasformula) | Indicates whether the text is formula if it starts with "=". |
| [setAttachedFilesDirectory()](#setattachedfilesdirectory) | The directory that the attached files will be saved to. NOTE: This member is now obsolete. Instead, please use HtmlLoadO |
| [setAutoFilter()](#setautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [setAutoFitColsAndRows()](#setautofitcolsandrows) | Indicates whether auto-fit columns and rows. The default value is false. |
| [setAutoFitterOptions()](#setautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [setCheckDataValid()](#setcheckdatavalid) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [setConvertDateTimeData()](#setconvertdatetimedata) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertFormulasData()](#setconvertformulasdata) | if true, convert string to formula when string value starts with character '=',the default value is false. NOTE: This pr |
| [setConvertNumericData()](#setconvertnumericdata) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [setDeleteRedundantSpaces()](#setdeleteredundantspaces) | Indicates whether delete redundant spaces when the text wraps lines using tag. The default value is false. |
| [setDetectLaTeX()](#setdetectlatex) |  |
| [setEncoding()](#setencoding) | Gets and sets the default encoding. Only applies for csv file. |
| [setFontConfigs()](#setfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [setHasFormula()](#sethasformula) | Indicates whether the text is formula if it starts with "=". |
| [setHyperlinkLoadMode()](#sethyperlinkloadmode) | The value of the property is HyperlinkLoadMode integer constant. |
| [setIgnoreNotPrinted()](#setignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [setIgnoreUselessShapes()](#setignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [setInterruptMonitor()](#setinterruptmonitor) | Gets and sets the interrupt monitor. |
| [setKeepPrecision()](#setkeepprecision) | Indicates whether not parsing a string value if the length is 15. |
| [setKeepUnparsedData()](#setkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [setLanguageCode()](#setlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [setLightCellsDataHandler()](#setlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [setLoadFilter()](#setloadfilter) | The filter to denote how to load data. |
| [setLoadFormulas()](#setloadformulas) | Indicates whether importing formulas if the original html file contains formulas |
| [setLoadStyleStrategy()](#setloadstylestrategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of |
| [setLocale()](#setlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [setMemorySetting()](#setmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [setPaperSize(type)](#setpapersize) | Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will  |
| [setParagrahLayoutMode()](#setparagrahlayoutmode) | The value of the property is HtmlParagraphLayoutMode integer constant. |
| [setParsingFormulaOnOpen()](#setparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [setParsingPivotCachedRecords()](#setparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [setPassword()](#setpassword) | Gets and set the password of the workbook. |
| [setPreservePaddingSpacesInFormula()](#setpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [setRegion()](#setregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [setStandardFont()](#setstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [setStandardFontSize()](#setstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [setSupportDivTag()](#setsupportdivtag) | Indicates whether support the layout of tag when the html file contains it. The default value is false. |
| [setWarningCallback()](#setwarningcallback) | Gets or sets warning callback. |

### constructor_overload$1(loadFormat) {#constructor-overload1}

Creates an options of loading the file.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | LoadFormat |

### getAttachedFilesDirectory() {#getattachedfilesdirectory}

The directory that the attached files will be saved to. NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

### getAutoFilter() {#getautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### getAutoFitColsAndRows() {#getautofitcolsandrows}

Indicates whether auto-fit columns and rows. The default value is false.

### getAutoFitterOptions() {#getautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### getCheckDataValid() {#getcheckdatavalid}

Check whether data is valid in the template file.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### getConvertDateTimeData() {#getconvertdatetimedata}

Gets or sets a value that indicates whether the string in text file is converted to date data.

### getConvertFormulasData() {#getconvertformulasdata}

if true, convert string to formula when string value starts with character '=',the default value is false. NOTE: This property is now obsolete. Instead, please use HtmlLoadOptions.HasFormula property. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

### getConvertNumericData() {#getconvertnumericdata}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

### getDefaultStyleSettings() {#getdefaultstylesettings}

Gets the default style settings for initializing styles of the workbook

### getDeleteRedundantSpaces() {#getdeleteredundantspaces}

Indicates whether delete redundant spaces when the text wraps lines using tag. The default value is false.

### getDetectLaTeX() {#getdetectlatex}

### getEncoding() {#getencoding}

Gets and sets the default encoding. Only applies for csv file.

### getFontConfigs() {#getfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### getHyperlinkLoadMode() {#gethyperlinkloadmode}

The value of the property is HyperlinkLoadMode integer constant.

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

### getLoadFormulas() {#getloadformulas}

Indicates whether importing formulas if the original html file contains formulas

### getLoadStyleStrategy() {#getloadstylestrategy}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of the property is TxtLoadStyleStrategy integer constant.

### getLocale() {#getlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### getMemorySetting() {#getmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### getParagrahLayoutMode() {#getparagrahlayoutmode}

The value of the property is HtmlParagraphLayoutMode integer constant.

### getParsingFormulaOnOpen() {#getparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### getParsingPivotCachedRecords() {#getparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### getPassword() {#getpassword}

Gets and set the password of the workbook.

### getPreservePaddingSpacesInFormula() {#getpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### getProgId() {#getprogid}

Gets the program id of creating the file. Only for MHT files.

### getRegion() {#getregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### getStandardFont() {#getstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getStandardFontSize() {#getstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getSupportDivTag() {#getsupportdivtag}

Indicates whether support the layout of tag when the html file contains it. The default value is false.

### getTableLoadOptions() {#gettableloadoptions}

Get the HtmlTableLoadOptionCollection instance

### getWarningCallback() {#getwarningcallback}

Gets or sets warning callback.

### hasFormula() {#hasformula}

Indicates whether the text is formula if it starts with "=".

### setAttachedFilesDirectory() {#setattachedfilesdirectory}

The directory that the attached files will be saved to. NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

### setAutoFilter() {#setautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### setAutoFitColsAndRows() {#setautofitcolsandrows}

Indicates whether auto-fit columns and rows. The default value is false.

### setAutoFitterOptions() {#setautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### setCheckDataValid() {#setcheckdatavalid}

Check whether data is valid in the template file.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### setConvertDateTimeData() {#setconvertdatetimedata}

Gets or sets a value that indicates whether the string in text file is converted to date data.

### setConvertFormulasData() {#setconvertformulasdata}

if true, convert string to formula when string value starts with character '=',the default value is false. NOTE: This property is now obsolete. Instead, please use HtmlLoadOptions.HasFormula property. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

### setConvertNumericData() {#setconvertnumericdata}

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

### setDeleteRedundantSpaces() {#setdeleteredundantspaces}

Indicates whether delete redundant spaces when the text wraps lines using tag. The default value is false.

### setDetectLaTeX() {#setdetectlatex}

### setEncoding() {#setencoding}

Gets and sets the default encoding. Only applies for csv file.

### setFontConfigs() {#setfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### setHasFormula() {#sethasformula}

Indicates whether the text is formula if it starts with "=".

### setHyperlinkLoadMode() {#sethyperlinkloadmode}

The value of the property is HyperlinkLoadMode integer constant.

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

### setLoadFormulas() {#setloadformulas}

Indicates whether importing formulas if the original html file contains formulas

### setLoadStyleStrategy() {#setloadstylestrategy}

Indicates the strategy to apply style for parsed values when converting string value to number or datetime. The value of the property is TxtLoadStyleStrategy integer constant.

### setLocale() {#setlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### setMemorySetting() {#setmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | PaperSizeType |

### setParagrahLayoutMode() {#setparagrahlayoutmode}

The value of the property is HtmlParagraphLayoutMode integer constant.

### setParsingFormulaOnOpen() {#setparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### setParsingPivotCachedRecords() {#setparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### setPassword() {#setpassword}

Gets and set the password of the workbook.

### setPreservePaddingSpacesInFormula() {#setpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### setRegion() {#setregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### setStandardFont() {#setstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setStandardFontSize() {#setstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setSupportDivTag() {#setsupportdivtag}

Indicates whether support the layout of tag when the html file contains it. The default value is false.

### setWarningCallback() {#setwarningcallback}

Gets or sets warning callback.
