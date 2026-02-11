---
title: Aspose::Cells::Numbers::NumbersLoadOptions class
linktitle: NumbersLoadOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Numbers::NumbersLoadOptions class. Represents the options of loading Apple Numbers files in C++.'
type: docs
weight: 100
url: /cpp/aspose.cells.numbers/numbersloadoptions/
---
## NumbersLoadOptions class


Represents the options of loading Apple [Numbers](../) files.

```cpp
class NumbersLoadOptions : public Aspose::Cells::LoadOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetAutoFilter()](../../aspose.cells/loadoptions/getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetAutoFitterOptions()](../../aspose.cells/loadoptions/getautofitteroptions/) | Gets and sets the auto fitter options. |
| [GetCheckDataValid()](../../aspose.cells/loadoptions/getcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction()](../../aspose.cells/loadoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetDefaultStyleSettings()](../../aspose.cells/loadoptions/getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook. |
| [GetFontConfigs()](../../aspose.cells/loadoptions/getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../../aspose.cells/workbook/) which uses this [LoadOptions](../../aspose.cells/loadoptions/) to load. |
| [GetIgnoreNotPrinted()](../../aspose.cells/loadoptions/getignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [GetIgnoreUselessShapes()](../../aspose.cells/loadoptions/getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetInterruptMonitor()](../../aspose.cells/loadoptions/getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetKeepUnparsedData()](../../aspose.cells/loadoptions/getkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../../aspose.cells/workbook/) when it is loaded from template file. Default is true. |
| [GetLanguageCode()](../../aspose.cells/loadoptions/getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../../aspose.cells/workbook/) version based on CountryCode that has saved the file. |
| [GetLightCellsDataHandler()](../../aspose.cells/loadoptions/getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [GetLoadFilter()](../../aspose.cells/loadoptions/getloadfilter/) | The filter to denote how to load data. |
| [GetLoadFormat()](../../aspose.cells/loadoptions/getloadformat/) | Gets the load format. |
| [GetLoadTableType()](./getloadtabletype/) | Gets and sets the type of loading multiple tables in one worksheet. |
| [GetMemorySetting()](../../aspose.cells/loadoptions/getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](../../aspose.cells/loadoptions/getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](../../aspose.cells/loadoptions/getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](../../aspose.cells/loadoptions/getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](../../aspose.cells/loadoptions/getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetPreserveTableName()](./getpreservetablename/) | Indicates whether to preserve table names when importing from [Numbers](../). |
| [GetRegion()](../../aspose.cells/loadoptions/getregion/) | Gets or sets the regional settings used for the [Workbook](../../aspose.cells/workbook/) that will be loaded. |
| [GetWarningCallback()](../../aspose.cells/loadoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadOptions()](../../aspose.cells/loadoptions/loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](../../aspose.cells/loadoptions/loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](../../aspose.cells/loadoptions/loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](../../aspose.cells/loadoptions/loadoptions/) | Copy constructor. |
| [NumbersLoadOptions()](./numbersloadoptions/) | Constructor. |
| [NumbersLoadOptions(NumbersLoadOptions_Impl* impl)](./numbersloadoptions/) | Constructs from an implementation object. |
| [NumbersLoadOptions(const NumbersLoadOptions\& src)](./numbersloadoptions/) | Copy constructor. |
| [NumbersLoadOptions(const LoadOptions\& src)](./numbersloadoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const NumbersLoadOptions\& src)](./operator_asm/) | operator= |
| [operator=(const LoadOptions\& src)](../../aspose.cells/loadoptions/operator_asm/) | operator= |
| [SetAutoFilter(bool value)](../../aspose.cells/loadoptions/setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](../../aspose.cells/loadoptions/setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](../../aspose.cells/loadoptions/setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](../../aspose.cells/loadoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](../../aspose.cells/loadoptions/setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../../aspose.cells/workbook/) which uses this [LoadOptions](../../aspose.cells/loadoptions/) to load. |
| [SetIgnoreNotPrinted(bool value)](../../aspose.cells/loadoptions/setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreUselessShapes(bool value)](../../aspose.cells/loadoptions/setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](../../aspose.cells/loadoptions/setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetKeepUnparsedData(bool value)](../../aspose.cells/loadoptions/setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../../aspose.cells/workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](../../aspose.cells/loadoptions/setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../../aspose.cells/workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](../../aspose.cells/loadoptions/setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](../../aspose.cells/loadoptions/setloadfilter/) | The filter to denote how to load data. |
| [SetLoadTableType(LoadNumbersTableType value)](./setloadtabletype/) | Gets and sets the type of loading multiple tables in one worksheet. |
| [SetMemorySetting(MemorySetting value)](../../aspose.cells/loadoptions/setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetPaperSize(PaperSizeType type)](../../aspose.cells/loadoptions/setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](../../aspose.cells/loadoptions/setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](../../aspose.cells/loadoptions/setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](../../aspose.cells/loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](../../aspose.cells/loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](../../aspose.cells/loadoptions/setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetPreserveTableName(bool value)](./setpreservetablename/) | Indicates whether to preserve table names when importing from [Numbers](../). |
| [SetRegion(CountryCode value)](../../aspose.cells/loadoptions/setregion/) | Gets or sets the regional settings used for the [Workbook](../../aspose.cells/workbook/) that will be loaded. |
| [SetWarningCallback(IWarningCallback* value)](../../aspose.cells/loadoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~LoadOptions()](../../aspose.cells/loadoptions/~loadoptions/) | Destructor. |
| [~NumbersLoadOptions()](./~numbersloadoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [LoadOptions](../../aspose.cells/loadoptions/)
* Namespace [Aspose::Cells::Numbers](../)
* Library [Aspose.Cells for C++](../../)
