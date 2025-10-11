---
title: Aspose::Cells::MarkdownLoadOptions class
linktitle: MarkdownLoadOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::MarkdownLoadOptions class. Represents the options for loading markdown document in C++.'
type: docs
weight: 10200
url: /cpp/aspose.cells/markdownloadoptions/
---
## MarkdownLoadOptions class


Represents the options for loading markdown document.

```cpp
class MarkdownLoadOptions : public Aspose::Cells::AbstractTextLoadOptions
```

## Methods

| Method | Description |
| --- | --- |
| [AbstractTextLoadOptions(AbstractTextLoadOptions_Impl* impl)](../abstracttextloadoptions/abstracttextloadoptions/) | Constructs from an implementation object. |
| [AbstractTextLoadOptions(const AbstractTextLoadOptions\& src)](../abstracttextloadoptions/abstracttextloadoptions/) | Copy constructor. |
| [AbstractTextLoadOptions(const LoadOptions\& src)](../abstracttextloadoptions/abstracttextloadoptions/) | Constructs from a parent object. |
| [GetAutoFilter()](../loadoptions/getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetAutoFitterOptions()](../loadoptions/getautofitteroptions/) | Gets and sets the auto fitter options. |
| [GetCheckDataValid()](../loadoptions/getcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction()](../loadoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetConvertDateTimeData()](../abstracttextloadoptions/getconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [GetConvertNumericData()](../abstracttextloadoptions/getconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [GetDefaultStyleSettings()](../loadoptions/getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook. |
| [GetEncoding()](../abstracttextloadoptions/getencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [GetFontConfigs()](../loadoptions/getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [GetHasFormula()](./gethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [GetIgnoreNotPrinted()](../loadoptions/getignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [GetIgnoreUselessShapes()](../loadoptions/getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetInterruptMonitor()](../loadoptions/getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetKeepPrecision()](../abstracttextloadoptions/getkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [GetKeepUnparsedData()](../loadoptions/getkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [GetLanguageCode()](../loadoptions/getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [GetLightCellsDataHandler()](../loadoptions/getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [GetLoadFilter()](../loadoptions/getloadfilter/) | The filter to denote how to load data. |
| [GetLoadFormat()](../loadoptions/getloadformat/) | Gets the load format. |
| [GetLoadStyleStrategy()](../abstracttextloadoptions/getloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [GetMemorySetting()](../loadoptions/getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](../loadoptions/getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](../loadoptions/getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](../loadoptions/getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](../loadoptions/getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetRegion()](../loadoptions/getregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [GetWarningCallback()](../loadoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadOptions()](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](../loadoptions/loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](../loadoptions/loadoptions/) | Copy constructor. |
| [MarkdownLoadOptions()](./markdownloadoptions/) | Default constructor. |
| [MarkdownLoadOptions(MarkdownLoadOptions_Impl* impl)](./markdownloadoptions/) | Constructs from an implementation object. |
| [MarkdownLoadOptions(const MarkdownLoadOptions\& src)](./markdownloadoptions/) | Copy constructor. |
| [MarkdownLoadOptions(const AbstractTextLoadOptions\& src)](./markdownloadoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const MarkdownLoadOptions\& src)](./operator_asm/) | operator= |
| [operator=(const AbstractTextLoadOptions\& src)](../abstracttextloadoptions/operator_asm/) | operator= |
| [operator=(const LoadOptions\& src)](../loadoptions/operator_asm/) | operator= |
| [SetAutoFilter(bool value)](../loadoptions/setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](../loadoptions/setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](../loadoptions/setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](../loadoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetConvertDateTimeData(bool value)](../abstracttextloadoptions/setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [SetConvertNumericData(bool value)](../abstracttextloadoptions/setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [SetEncoding(EncodingType value)](../abstracttextloadoptions/setencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](../loadoptions/setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [SetHasFormula(bool value)](./sethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [SetIgnoreNotPrinted(bool value)](../loadoptions/setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreUselessShapes(bool value)](../loadoptions/setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](../loadoptions/setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetKeepPrecision(bool value)](../abstracttextloadoptions/setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [SetKeepUnparsedData(bool value)](../loadoptions/setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](../loadoptions/setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](../loadoptions/setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](../loadoptions/setloadfilter/) | The filter to denote how to load data. |
| [SetLoadStyleStrategy(TxtLoadStyleStrategy value)](../abstracttextloadoptions/setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [SetMemorySetting(MemorySetting value)](../loadoptions/setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetPaperSize(PaperSizeType type)](../loadoptions/setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](../loadoptions/setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](../loadoptions/setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](../loadoptions/setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetRegion(CountryCode value)](../loadoptions/setregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [SetWarningCallback(IWarningCallback* value)](../loadoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~AbstractTextLoadOptions()](../abstracttextloadoptions/~abstracttextloadoptions/) | Destructor. |
| [~LoadOptions()](../loadoptions/~loadoptions/) | Destructor. |
| [~MarkdownLoadOptions()](./~markdownloadoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
