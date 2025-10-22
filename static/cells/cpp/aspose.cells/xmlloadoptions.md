##Aspose::Cells::XmlLoadOptions class
'Aspose::Cells::XmlLoadOptions class. Represents the options of loading xml in C++.'
## XmlLoadOptions class
Represents the options of loading xml.
```cpp
class XmlLoadOptions : public Aspose::Cells::LoadOptions
```
## Methods
| Method | Description |
| --- | --- |
| [Get_DateFormat()](./get_dateformat/) | Gets and sets the format of date value. |
| [Get_NumberFormat()](./get_numberformat/) | Gets and sets the format of numeric value. |
| [GetAutoFilter()](../loadoptions/getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetAutoFitterOptions()](../loadoptions/getautofitteroptions/) | Gets and sets the auto fitter options. |
| [GetCheckDataValid()](../loadoptions/getcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction()](../loadoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetContainsMultipleWorksheets()](./getcontainsmultipleworksheets/) | Indicates whether importing xml as multiple worksheets. |
| [GetConvertNumericOrDate()](./getconvertnumericordate/) | Indicates whether converting the value in xml file to numeric or date. |
| [GetDefaultStyleSettings()](../loadoptions/getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook. |
| [GetFontConfigs()](../loadoptions/getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [GetIgnoreNotPrinted()](../loadoptions/getignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [GetIgnoreRootAttributes()](./getignorerootattributes/) | Indicates whether ignore attributes of the root element. |
| [GetIgnoreUselessShapes()](../loadoptions/getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetInterruptMonitor()](../loadoptions/getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetKeepUnparsedData()](../loadoptions/getkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [GetLanguageCode()](../loadoptions/getlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [GetLightCellsDataHandler()](../loadoptions/getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [GetLoadFilter()](../loadoptions/getloadfilter/) | The filter to denote how to load data. |
| [GetLoadFormat()](../loadoptions/getloadformat/) | Gets the load format. |
| [GetMemorySetting()](../loadoptions/getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](../loadoptions/getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](../loadoptions/getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](../loadoptions/getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](../loadoptions/getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetRegion()](../loadoptions/getregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [GetStartCell()](./getstartcell/) | Gets and sets the start cell. |
| [GetWarningCallback()](../loadoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsXmlMap()](./isxmlmap/) | Indicates whether mapping xml to Excel. The default value is false. |
| [LoadOptions()](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](../loadoptions/loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](../loadoptions/loadoptions/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const XmlLoadOptions\& src)](./operator_asm/) | operator= |
| [operator=(const LoadOptions\& src)](../loadoptions/operator_asm/) | operator= |
| [SetAutoFilter(bool value)](../loadoptions/setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](../loadoptions/setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](../loadoptions/setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](../loadoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetContainsMultipleWorksheets(bool value)](./setcontainsmultipleworksheets/) | Indicates whether importing xml as multiple worksheets. |
| [SetConvertNumericOrDate(bool value)](./setconvertnumericordate/) | Indicates whether converting the value in xml file to numeric or date. |
| [SetDateFormat(const U16String\& value)](./setdateformat/) | Gets and sets the format of date value. |
| [SetDateFormat(const char16_t* value)](./setdateformat/) | Gets and sets the format of date value. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](../loadoptions/setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [SetIgnoreNotPrinted(bool value)](../loadoptions/setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreRootAttributes(bool value)](./setignorerootattributes/) | Indicates whether ignore attributes of the root element. |
| [SetIgnoreUselessShapes(bool value)](../loadoptions/setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](../loadoptions/setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetIsXmlMap(bool value)](./setisxmlmap/) | Indicates whether mapping xml to Excel. The default value is false. |
| [SetKeepUnparsedData(bool value)](../loadoptions/setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](../loadoptions/setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](../loadoptions/setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](../loadoptions/setloadfilter/) | The filter to denote how to load data. |
| [SetMemorySetting(MemorySetting value)](../loadoptions/setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetNumberFormat(const U16String\& value)](./setnumberformat/) | Gets and sets the format of numeric value. |
| [SetNumberFormat(const char16_t* value)](./setnumberformat/) | Gets and sets the format of numeric value. |
| [SetPaperSize(PaperSizeType type)](../loadoptions/setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](../loadoptions/setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](../loadoptions/setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](../loadoptions/setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetRegion(CountryCode value)](../loadoptions/setregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [SetStartCell(const U16String\& value)](./setstartcell/) | Gets and sets the start cell. |
| [SetStartCell(const char16_t* value)](./setstartcell/) | Gets and sets the start cell. |
| [SetWarningCallback(IWarningCallback* value)](../loadoptions/setwarningcallback/) | Gets or sets warning callback. |
| [XmlLoadOptions()](./xmlloadoptions/) | Represents the options of loading xml file. |
| explicit [XmlLoadOptions(LoadFormat type)](./xmlloadoptions/) | Represents the options of loading xml file. |
| [XmlLoadOptions(XmlLoadOptions_Impl* impl)](./xmlloadoptions/) | Constructs from an implementation object. |
| [XmlLoadOptions(const XmlLoadOptions\& src)](./xmlloadoptions/) | Copy constructor. |
| [XmlLoadOptions(const LoadOptions\& src)](./xmlloadoptions/) | Constructs from a parent object. |
| [~LoadOptions()](../loadoptions/~loadoptions/) | Destructor. |
| [~XmlLoadOptions()](./~xmlloadoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [LoadOptions](../loadoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
