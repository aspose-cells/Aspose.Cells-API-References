##Aspose::Cells::TxtLoadOptions class
'Aspose::Cells::TxtLoadOptions class. Represents the options for loading text file in C++.'
## TxtLoadOptions class
Represents the options for loading text file.
```cpp
class TxtLoadOptions : public Aspose::Cells::AbstractTextLoadOptions
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
| [GetExtendToNextSheet()](./getextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [GetFontConfigs()](../loadoptions/getfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [GetHasFormula()](./gethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [GetHasTextQualifier()](./gethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. |
| [GetHeaderColumnsCount()](./getheadercolumnscount/) | The count of header columns to be repeated for extended sheets. |
| [GetHeaderRowsCount()](./getheaderrowscount/) | The count of header rows to be repeated for extended sheets. |
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
| [GetMaxColumnCount()](./getmaxcolumncount/) | The maximum count of columns to be imported for one sheet. |
| [GetMaxRowCount()](./getmaxrowcount/) | The maximum count of rows to be imported for one sheet. |
| [GetMemorySetting()](../loadoptions/getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetParsingFormulaOnOpen()](../loadoptions/getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords()](../loadoptions/getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [GetPassword()](../loadoptions/getpassword/) | Gets and set the password of the workbook. |
| [GetPreservePaddingSpacesInFormula()](../loadoptions/getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [GetRegion()](../loadoptions/getregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [GetSeparator()](./getseparator/) | Gets and sets character separator of text file. |
| [GetSeparatorString()](./getseparatorstring/) | Gets and sets a string value as separator. |
| [GetTextQualifier()](./gettextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [GetTreatConsecutiveDelimitersAsOne()](./gettreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. |
| [GetTreatQuotePrefixAsValue()](./gettreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and Style.QuotePrefix will be set as true for the cell. |
| [GetWarningCallback()](../loadoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsMultiEncoded()](./ismultiencoded/) | True means that the file contains several encoding. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LoadOptions()](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| explicit [LoadOptions(LoadFormat loadFormat)](../loadoptions/loadoptions/) | Creates an options of loading the file. |
| [LoadOptions(LoadOptions_Impl* impl)](../loadoptions/loadoptions/) | Constructs from an implementation object. |
| [LoadOptions(const LoadOptions\& src)](../loadoptions/loadoptions/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TxtLoadOptions\& src)](./operator_asm/) | operator= |
| [operator=(const AbstractTextLoadOptions\& src)](../abstracttextloadoptions/operator_asm/) | operator= |
| [operator=(const LoadOptions\& src)](../loadoptions/operator_asm/) | operator= |
| [SetAutoFilter(bool value)](../loadoptions/setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFitterOptions(const AutoFitterOptions\& value)](../loadoptions/setautofitteroptions/) | Gets and sets the auto fitter options. |
| [SetCheckDataValid(bool value)](../loadoptions/setcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckExcelRestriction(bool value)](../loadoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetConvertDateTimeData(bool value)](../abstracttextloadoptions/setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true. |
| [SetConvertNumericData(bool value)](../abstracttextloadoptions/setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true. |
| [SetEncoding(EncodingType value)](../abstracttextloadoptions/setencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [SetExtendToNextSheet(bool value)](./setextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [SetFontConfigs(const IndividualFontConfigs\& value)](../loadoptions/setfontconfigs/) | Gets and sets individual font configs. Only works for the [Workbook](../workbook/) which uses this [LoadOptions](../loadoptions/) to load. |
| [SetHasFormula(bool value)](./sethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [SetHasTextQualifier(bool value)](./sethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. |
| [SetHeaderColumnsCount(int32_t value)](./setheadercolumnscount/) | The count of header columns to be repeated for extended sheets. |
| [SetHeaderRowsCount(int32_t value)](./setheaderrowscount/) | The count of header rows to be repeated for extended sheets. |
| [SetIgnoreNotPrinted(bool value)](../loadoptions/setignorenotprinted/) | Ignore the data which are not printed if directly printing the file. |
| [SetIgnoreUselessShapes(bool value)](../loadoptions/setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](../loadoptions/setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetIsMultiEncoded(bool value)](./setismultiencoded/) | True means that the file contains several encoding. |
| [SetKeepPrecision(bool value)](../abstracttextloadoptions/setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [SetKeepUnparsedData(bool value)](../loadoptions/setkeepunparseddata/) | Whether keep the unparsed data in memory for the [Workbook](../workbook/) when it is loaded from template file. Default is true. |
| [SetLanguageCode(CountryCode value)](../loadoptions/setlanguagecode/) | Gets or sets the user interface language of the [Workbook](../workbook/) version based on CountryCode that has saved the file. |
| [SetLightCellsDataHandler(LightCellsDataHandler* value)](../loadoptions/setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [SetLoadFilter(LoadFilter* value)](../loadoptions/setloadfilter/) | The filter to denote how to load data. |
| [SetLoadStyleStrategy(TxtLoadStyleStrategy value)](../abstracttextloadoptions/setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [SetMaxColumnCount(int32_t value)](./setmaxcolumncount/) | The maximum count of columns to be imported for one sheet. |
| [SetMaxRowCount(int32_t value)](./setmaxrowcount/) | The maximum count of rows to be imported for one sheet. |
| [SetMemorySetting(MemorySetting value)](../loadoptions/setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetPaperSize(PaperSizeType type)](../loadoptions/setpapersize/) | Sets the default print paper size from default printer's setting. |
| [SetParsingFormulaOnOpen(bool value)](../loadoptions/setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingPivotCachedRecords(bool value)](../loadoptions/setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [SetPassword(const U16String\& value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPassword(const char16_t* value)](../loadoptions/setpassword/) | Gets and set the password of the workbook. |
| [SetPreservePaddingSpacesInFormula(bool value)](../loadoptions/setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [SetRegion(CountryCode value)](../loadoptions/setregion/) | Gets or sets the regional settings used for the [Workbook](../workbook/) that will be loaded. |
| [SetSeparator(char16_t value)](./setseparator/) | Gets and sets character separator of text file. |
| [SetSeparatorString(const U16String\& value)](./setseparatorstring/) | Gets and sets a string value as separator. |
| [SetSeparatorString(const char16_t* value)](./setseparatorstring/) | Gets and sets a string value as separator. |
| [SetTextQualifier(char16_t value)](./settextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [SetTreatConsecutiveDelimitersAsOne(bool value)](./settreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. |
| [SetTreatQuotePrefixAsValue(bool value)](./settreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and Style.QuotePrefix will be set as true for the cell. |
| [SetWarningCallback(IWarningCallback* value)](../loadoptions/setwarningcallback/) | Gets or sets warning callback. |
| [TxtLoadOptions()](./txtloadoptions/) | Creates the options for loading text file. |
| explicit [TxtLoadOptions(LoadFormat loadFormat)](./txtloadoptions/) | Creates the options for loading text file. |
| [TxtLoadOptions(TxtLoadOptions_Impl* impl)](./txtloadoptions/) | Constructs from an implementation object. |
| [TxtLoadOptions(const TxtLoadOptions\& src)](./txtloadoptions/) | Copy constructor. |
| [TxtLoadOptions(const AbstractTextLoadOptions\& src)](./txtloadoptions/) | Constructs from a parent object. |
| [~AbstractTextLoadOptions()](../abstracttextloadoptions/~abstracttextloadoptions/) | Destructor. |
| [~LoadOptions()](../loadoptions/~loadoptions/) | Destructor. |
| [~TxtLoadOptions()](./~txtloadoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
