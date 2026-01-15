---
title: Aspose::Cells::EbookLoadOptions class
linktitle: EbookLoadOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::EbookLoadOptions class. Represents options when importing an ebook file in C++.'
type: docs
weight: 5400
url: /cpp/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class


Represents options when importing an ebook file.

```cpp
class EbookLoadOptions : public Aspose::Cells::HtmlLoadOptions
```

## Methods

| Method | Description |
| --- | --- |
| [AbstractTextLoadOptions(AbstractTextLoadOptions_Impl* impl)](../abstracttextloadoptions/abstracttextloadoptions/) | Constructs from an implementation object. |
| [AbstractTextLoadOptions(const AbstractTextLoadOptions\& src)](../abstracttextloadoptions/abstracttextloadoptions/) | Copy constructor. |
| [AbstractTextLoadOptions(const LoadOptions\& src)](../abstracttextloadoptions/abstracttextloadoptions/) | Constructs from a parent object. |
| [EbookLoadOptions()](./ebookloadoptions/) | Creates an option for loading the ebook file. |
| explicit [EbookLoadOptions(LoadFormat loadFormat)](./ebookloadoptions/) | Creates an option of loading the ebook file. |
| [EbookLoadOptions(EbookLoadOptions_Impl* impl)](./ebookloadoptions/) | Constructs from an implementation object. |
| [EbookLoadOptions(const EbookLoadOptions\& src)](./ebookloadoptions/) | Copy constructor. |
| [EbookLoadOptions(const HtmlLoadOptions\& src)](./ebookloadoptions/) | Constructs from a parent object. |
| [GetAutoFilter()](../loadoptions/getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetAutoFitColsAndRows()](../htmlloadoptions/getautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. |
| [GetAutoFitterOptions()](../loadoptions/getautofitteroptions/) | Gets and sets the auto fitter options. |
| [GetCheckDataValid()](../loadoptions/getcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction()](../loadoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetConvertDateTimeData()](../abstracttextloadoptions/getconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [GetConvertNumericData()](../abstracttextloadoptions/getconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [GetDefaultStyleSettings()](../loadoptions/getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook. |
| [GetDeleteRedundantSpaces()](../htmlloadoptions/getdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using **<br>** tag. The default value is false. |
| [GetDetectLaTeX()](../htmlloadoptions/getdetectlatex/) | Indicates whether to detect LaTeX formula in the HTML file. The default value is false. |
| [GetEncoding()](../abstracttextloadoptions/getencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [GetFontConfigs()](../loadoptions/getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [GetHasFormula()](../htmlloadoptions/gethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [GetIgnoreNotPrinted()](../loadoptions/getignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [GetIgnoreUselessShapes()](../loadoptions/getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetInterruptMonitor()](../loadoptions/getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetKeepPrecision()](../abstracttextloadoptions/getkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [GetKeepUnparsedData()](../loadoptions/getkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [GetLanguageCode()](../loadoptions/getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [GetLightCellsDataHandler()](../loadoptions/getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [GetLoadFilter()](../loadoptions/getloadfilter/) | The filter to denote how to load data. |
| [GetLoadFormat()](../loadoptions/getloadformat/) | Gets the load format. |
| [GetLoadFormulas()](../htmlloadoptions/getloadformulas/) | Indicates whether importing formulas if the original html file contains formulas. |
| [GetLoadStyleStrategy()](../abstracttextloadoptions/getloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [GetMemorySetting()](../loadoptions/getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](../loadoptions/getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](../loadoptions/getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](../loadoptions/getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](../loadoptions/getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetProgId()](../htmlloadoptions/getprogid/) | Gets the program id of creating the file. Only for MHT files. |
| [GetRegion()](../loadoptions/getregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [GetSupportDivTag()](../htmlloadoptions/getsupportdivtag/) | Indicates whether support the layout of **<div>** tag when the html file contains it. The default value is false. |
| [GetTableLoadOptions()](../htmlloadoptions/gettableloadoptions/) | Get the [HtmlTableLoadOptionCollection](../htmltableloadoptioncollection/) instance. |
| [GetWarningCallback()](../loadoptions/getwarningcallback/) | Gets or sets warning callback. |
| [HtmlLoadOptions()](../htmlloadoptions/htmlloadoptions/) | Creates an options of loading the file. |
| explicit [HtmlLoadOptions(LoadFormat loadFormat)](../htmlloadoptions/htmlloadoptions/) | Creates an options of loading the file. |
| [HtmlLoadOptions(HtmlLoadOptions_Impl* impl)](../htmlloadoptions/htmlloadoptions/) | Constructs from an implementation object. |
| [HtmlLoadOptions(const HtmlLoadOptions\& src)](../htmlloadoptions/htmlloadoptions/) | Copy constructor. |
| [HtmlLoadOptions(const AbstractTextLoadOptions\& src)](../htmlloadoptions/htmlloadoptions/) | Constructs from a parent object. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadOptions()](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](../loadoptions/loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](../loadoptions/loadoptions/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const EbookLoadOptions\& src)](./operator_asm/) | operator= |
| [operator=(const HtmlLoadOptions\& src)](../htmlloadoptions/operator_asm/) | operator= |
| [operator=(const AbstractTextLoadOptions\& src)](../abstracttextloadoptions/operator_asm/) | operator= |
| [operator=(const LoadOptions\& src)](../loadoptions/operator_asm/) | operator= |
| [SetAutoFilter(bool value)](../loadoptions/setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitColsAndRows(bool value)](../htmlloadoptions/setautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](../loadoptions/setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](../loadoptions/setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](../loadoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetConvertDateTimeData(bool value)](../abstracttextloadoptions/setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [SetConvertNumericData(bool value)](../abstracttextloadoptions/setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [SetDeleteRedundantSpaces(bool value)](../htmlloadoptions/setdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using **<br>** tag. The default value is false. |
| [SetDetectLaTeX(bool value)](../htmlloadoptions/setdetectlatex/) | Indicates whether to detect LaTeX formula in the HTML file. The default value is false. |
| [SetEncoding(EncodingType value)](../abstracttextloadoptions/setencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](../loadoptions/setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [SetHasFormula(bool value)](../htmlloadoptions/sethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [SetIgnoreNotPrinted(bool value)](../loadoptions/setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreUselessShapes(bool value)](../loadoptions/setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](../loadoptions/setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetKeepPrecision(bool value)](../abstracttextloadoptions/setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [SetKeepUnparsedData(bool value)](../loadoptions/setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](../loadoptions/setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](../loadoptions/setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](../loadoptions/setloadfilter/) | The filter to denote how to load data. |
| [SetLoadFormulas(bool value)](../htmlloadoptions/setloadformulas/) | Indicates whether importing formulas if the original html file contains formulas. |
| [SetLoadStyleStrategy(TxtLoadStyleStrategy value)](../abstracttextloadoptions/setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [SetMemorySetting(MemorySetting value)](../loadoptions/setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetPaperSize(PaperSizeType type)](../loadoptions/setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](../loadoptions/setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](../loadoptions/setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](../loadoptions/setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetRegion(CountryCode value)](../loadoptions/setregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [SetSupportDivTag(bool value)](../htmlloadoptions/setsupportdivtag/) | Indicates whether support the layout of **<div>** tag when the html file contains it. The default value is false. |
| [SetWarningCallback(IWarningCallback* value)](../loadoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~AbstractTextLoadOptions()](../abstracttextloadoptions/~abstracttextloadoptions/) | Destructor. |
| [~EbookLoadOptions()](./~ebookloadoptions/) | Destructor. |
| [~HtmlLoadOptions()](../htmlloadoptions/~htmlloadoptions/) | Destructor. |
| [~LoadOptions()](../loadoptions/~loadoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [HtmlLoadOptions](../htmlloadoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
