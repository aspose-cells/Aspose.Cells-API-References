##Aspose::Cells::LoadOptions class
'Aspose::Cells::LoadOptions class. Represents the options of loading the file in C++.'
## LoadOptions class
Represents the options of loading the file.
```cpp
class LoadOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAutoFilter()](./getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetAutoFitterOptions()](./getautofitteroptions/) | Gets and sets the auto fitter options. |
| [GetCheckDataValid()](./getcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction()](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetDefaultStyleSettings()](./getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook. |
| [GetFontConfigs()](./getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](./) to load. |
| [GetIgnoreNotPrinted()](./getignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [GetIgnoreUselessShapes()](./getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetInterruptMonitor()](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetKeepUnparsedData()](./getkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [GetLanguageCode()](./getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [GetLightCellsDataHandler()](./getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [GetLoadFilter()](./getloadfilter/) | The filter to denote how to load data. |
| [GetLoadFormat()](./getloadformat/) | Gets the load format. |
| [GetMemorySetting()](./getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](./getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](./getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](./getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](./getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetRegion()](./getregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [GetWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadOptions()](./loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](./loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](./loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](./loadoptions/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LoadOptions\& src)](./operator_asm/) | operator= |
| [SetAutoFilter(bool value)](./setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](./setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](./setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](./setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](./) to load. |
| [SetIgnoreNotPrinted(bool value)](./setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreUselessShapes(bool value)](./setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](./setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetKeepUnparsedData(bool value)](./setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](./setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](./setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](./setloadfilter/) | The filter to denote how to load data. |
| [SetMemorySetting(MemorySetting value)](./setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetPaperSize(PaperSizeType type)](./setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](./setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](./setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](./setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](./setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](./setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetRegion(CountryCode value)](./setregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [SetWarningCallback(IWarningCallback* value)](./setwarningcallback/) | Gets or sets warning callback. |
| [~LoadOptions()](./~loadoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
