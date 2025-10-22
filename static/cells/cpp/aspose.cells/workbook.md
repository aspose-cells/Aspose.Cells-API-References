##Aspose::Cells::Workbook class
'Aspose::Cells::Workbook class. Represents a root object to create an Excel spreadsheet in C++.'
## Workbook class
Represents a root object to create an Excel spreadsheet.
```cpp
class Workbook
```
## Methods
| Method | Description |
| --- | --- |
| [AcceptAllRevisions()](./acceptallrevisions/) | Accepts all tracked changes in the workbook. |
| [AddDigitalSignature(const DigitalSignatureCollection\& digitalSignatureCollection)](./adddigitalsignature/) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [CalculateFormula()](./calculateformula/) | Calculates the result of formulas. |
| [CalculateFormula(bool ignoreError)](./calculateformula/) | Calculates the result of formulas. |
| [CalculateFormula(const CalculationOptions\& options)](./calculateformula/) | Calculating formulas in this workbook. |
| [ChangePalette(const Aspose::Cells::Color\& color, int32_t index)](./changepalette/) | Changes the palette for the spreadsheet in the specified index. |
| [CloseAccessCache(AccessCacheOptions opts)](./closeaccesscache/) | Closes the session that uses caches to access data. |
| [Combine(const Workbook\& secondWorkbook)](./combine/) | Combines another [Workbook](./) object. |
| [Copy(const Workbook\& source, const CopyOptions\& copyOptions)](./copy/) | Copies another [Workbook](./) object. |
| [Copy(const Workbook\& source)](./copy/) | Copies data from a source [Workbook](./) object. |
| [CopyTheme(const Workbook\& source)](./copytheme/) | Copies the theme from another workbook. |
| [CreateBuiltinStyle(BuiltinStyleType type)](./createbuiltinstyle/) | Creates built-in style by given type. |
| [CreateCellsColor()](./createcellscolor/) | Creates a [CellsColor](../cellscolor/) object. |
| [CreateStyle()](./createstyle/) | Creates a new style. |
| [CreateStyle(bool cloneDefaultStyle)](./createstyle/) | Creates a new style. |
| [CustomTheme(const U16String\& themeName, const Vector \<Aspose::Cells::Color\>\& colors)](./customtheme/) | Customs the theme. |
| [CustomTheme(const char16_t* themeName, const Vector \<Aspose::Cells::Color\>\& colors)](./customtheme/) | Customs the theme. |
| [Dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExportXml(const U16String\& mapName, const U16String\& path)](./exportxml/) | Export XML data linked by the specified XML map. |
| [ExportXml(const char16_t* mapName, const char16_t* path)](./exportxml/) | Export XML data linked by the specified XML map. |
| [ExportXml(const U16String\& mapName)](./exportxml/) | Export XML data. |
| [ExportXml(const char16_t* mapName)](./exportxml/) | Export XML data. |
| [GetAbsolutePath()](./getabsolutepath/) | Gets and sets the absolute path of the file. |
| [GetBuiltInDocumentProperties()](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
| [GetColors()](./getcolors/) | Returns colors in the palette for the spreadsheet. |
| [GetContentTypeProperties()](./getcontenttypeproperties/) | Gets the list of ContentTypeProperty objects in the workbook. |
| [GetCountOfStylesInPool()](./getcountofstylesinpool/) | Gets number of the styles in the style pool. |
| [GetCustomDocumentProperties()](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [GetCustomXmlParts()](./getcustomxmlparts/) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [GetDataConnections()](./getdataconnections/) | Gets the ExternalConnection collection. |
| [GetDataMashup()](./getdatamashup/) | Gets mashup data. |
| [GetDataModel()](./getdatamodel/) | Gets data model in the workbook. |
| [GetDataSorter()](./getdatasorter/) | Gets a [DataSorter](../datasorter/) object to sort data. |
| [GetDefaultStyle()](./getdefaultstyle/) | Gets or sets the default [Style](../style/) object of the workbook. |
| [GetDigitalSignature()](./getdigitalsignature/) | Gets digital signature from file. |
| [GetFileFormat()](./getfileformat/) | Gets and sets the file format. |
| [GetFileName()](./getfilename/) | Gets and sets the current file name. |
| [GetFonts()](./getfonts/) | Gets all fonts in the style pool. |
| [GetHasCustomFunction()](./gethascustomfunction/) | Detects whether there is custom function used in this workbook, such as in cell's formula, in defined names... |
| [GetHasMacro()](./gethasmacro/) | Indicates if this spreadsheet contains macro/VBA. |
| [GetHasRevisions()](./gethasrevisions/) | Gets if the workbook has any tracked changes. |
| [GetInterruptMonitor()](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetMatchingColor(const Aspose::Cells::Color\& rawColor)](./getmatchingcolor/) | Find best matching [Color](../color/) in current palette. |
| [GetNamedStyle(const U16String\& name)](./getnamedstyle/) | Gets the named style in the style pool. |
| [GetNamedStyle(const char16_t* name)](./getnamedstyle/) | Gets the named style in the style pool. |
| [GetRibbonXml()](./getribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
| [GetSettings()](./getsettings/) | Represents the workbook settings. |
| [GetStyleInPool(int32_t index)](./getstyleinpool/) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. |
| [GetTheme()](./gettheme/) | Gets the theme name. |
| [GetThemeColor(ThemeColorType type)](./getthemecolor/) | Gets theme color. |
| [GetVbaProject()](./getvbaproject/) | Gets the VbaProject in a spreadsheet. |
| [GetWorksheets()](./getworksheets/) | Gets the [WorksheetCollection](../worksheetcollection/) collection in the spreadsheet. |
| [ImportXml(const U16String\& url, const U16String\& sheetName, int32_t row, int32_t col)](./importxml/) | Imports/Updates an XML data file into the workbook. |
| [ImportXml(const char16_t* url, const char16_t* sheetName, int32_t row, int32_t col)](./importxml/) | Imports/Updates an XML data file into the workbook. |
| [ImportXml(const Vector \<uint8_t\>\& stream, const U16String\& sheetName, int32_t row, int32_t col)](./importxml/) | Imports/Updates an XML data file into the workbook. |
| [ImportXml(const Vector \<uint8_t\>\& stream, const char16_t* sheetName, int32_t row, int32_t col)](./importxml/) | Imports/Updates an XML data file into the workbook. |
| [IsColorInPalette(const Aspose::Cells::Color\& color)](./iscolorinpalette/) | Checks if a color is in the palette for the spreadsheet. |
| [IsDigitallySigned()](./isdigitallysigned/) | Indicates if this spreadsheet is digitally signed. |
| [IsLicensed()](./islicensed/) | Indicates whether license is set. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsWorkbookProtectedWithPassword()](./isworkbookprotectedwithpassword/) | Indicates whether structure or window is protected with password. |
| [MergeNamedStyles(const Workbook\& source)](./mergenamedstyles/) | Merges named styles from the other Excel file. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Workbook\& src)](./operator_asm/) | operator= |
| [ParseFormulas(bool ignoreError)](./parseformulas/) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [Protect(ProtectionType protectionType, const U16String\& password)](./protect/) | Protects a workbook. |
| [Protect(ProtectionType protectionType, const char16_t* password)](./protect/) | Protects a workbook. |
| [ProtectSharedWorkbook(const U16String\& password)](./protectsharedworkbook/) | Protects a shared workbook. |
| [ProtectSharedWorkbook(const char16_t* password)](./protectsharedworkbook/) | Protects a shared workbook. |
| [RefreshDynamicArrayFormulas(bool calculate)](./refreshdynamicarrayformulas/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. |
| [RefreshDynamicArrayFormulas(bool calculate, const CalculationOptions\& copts)](./refreshdynamicarrayformulas/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [RemoveDigitalSignature()](./removedigitalsignature/) | Removes digital signature from this spreadsheet. |
| [RemoveMacro()](./removemacro/) | Removes VBA/macro from this spreadsheet. |
| [RemovePersonalInformation()](./removepersonalinformation/) | Removes personal information. |
| [RemoveUnusedStyles()](./removeunusedstyles/) | Remove all unused styles. |
| [Replace(const U16String\& placeHolder, const U16String\& newValue)](./replace/) | Replaces a cell's value with a new string. |
| [Replace(const char16_t* placeHolder, const char16_t* newValue)](./replace/) | Replaces a cell's value with a new string. |
| [Replace(const U16String\& placeHolder, int32_t newValue)](./replace/) | Replaces a cell's value with a new integer. |
| [Replace(const char16_t* placeHolder, int32_t newValue)](./replace/) | Replaces a cell's value with a new integer. |
| [Replace(const U16String\& placeHolder, double newValue)](./replace/) | Replaces a cell's value with a new double. |
| [Replace(const char16_t* placeHolder, double newValue)](./replace/) | Replaces a cell's value with a new double. |
| [Replace(const U16String\& placeHolder, const Vector \<U16String\>\& newValues, bool isVertical)](./replace/) | Replaces a cell's value with a new string array. |
| [Replace(const char16_t* placeHolder, const Vector \<U16String\>\& newValues, bool isVertical)](./replace/) | Replaces a cell's value with a new string array. |
| [Replace(const U16String\& placeHolder, const Vector \<int32_t\>\& newValues, bool isVertical)](./replace/) | Replaces cells' values with an integer array. |
| [Replace(const char16_t* placeHolder, const Vector \<int32_t\>\& newValues, bool isVertical)](./replace/) | Replaces cells' values with an integer array. |
| [Replace(const U16String\& placeHolder, const Vector \<double\>\& newValues, bool isVertical)](./replace/) | Replaces cells' values with a double array. |
| [Replace(const char16_t* placeHolder, const Vector \<double\>\& newValues, bool isVertical)](./replace/) | Replaces cells' values with a double array. |
| [Replace(bool boolValue, const Aspose::Cells::Object\& newValue)](./replace/) | Replaces cells' values with new data. |
| [Replace(int32_t intValue, const Aspose::Cells::Object\& newValue)](./replace/) | Replaces cells' values with new data. |
| [Replace(const U16String\& placeHolder, const U16String\& newValue, const ReplaceOptions\& options)](./replace/) | Replaces a cell's value with a new string. |
| [Replace(const char16_t* placeHolder, const char16_t* newValue, const ReplaceOptions\& options)](./replace/) | Replaces a cell's value with a new string. |
| [Save(const U16String\& fileName, SaveFormat saveFormat)](./save/) | Saves the workbook to the disk. |
| [Save(const char16_t* fileName, SaveFormat saveFormat)](./save/) | Saves the workbook to the disk. |
| [Save(const U16String\& fileName)](./save/) | Save the workbook to the disk. |
| [Save(const char16_t* fileName)](./save/) | Save the workbook to the disk. |
| [Save(const U16String\& fileName, const SaveOptions\& saveOptions)](./save/) | Saves the workbook to the disk. |
| [Save(const char16_t* fileName, const SaveOptions\& saveOptions)](./save/) | Saves the workbook to the disk. |
| [Save(SaveFormat saveFormat)](./save/) | Saves the workbook to the stream. |
| [Save(const SaveOptions\& saveOptions)](./save/) | Saves the workbook to the stream. |
| [SaveToStream()](./savetostream/) | Saves Excel file to a MemoryStream object as an Excel97-2003 xls file and returns it. |
| [SetAbsolutePath(const U16String\& value)](./setabsolutepath/) | Gets and sets the absolute path of the file. |
| [SetAbsolutePath(const char16_t* value)](./setabsolutepath/) | Gets and sets the absolute path of the file. |
| [SetDefaultStyle(const Style\& value)](./setdefaultstyle/) | Gets or sets the default [Style](../style/) object of the workbook. |
| [SetDigitalSignature(const DigitalSignatureCollection\& digitalSignatureCollection)](./setdigitalsignature/) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [SetEncryptionOptions(EncryptionType encryptionType, int32_t keyLength)](./setencryptionoptions/) | Set Encryption Options. |
| [SetFileFormat(FileFormatType value)](./setfileformat/) | Gets and sets the file format. |
| [SetFileName(const U16String\& value)](./setfilename/) | Gets and sets the current file name. |
| [SetFileName(const char16_t* value)](./setfilename/) | Gets and sets the current file name. |
| [SetInterruptMonitor(AbstractInterruptMonitor* value)](./setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetInterruptMonitor(const InterruptMonitor\& interruptMonitor)](./setinterruptmonitor/) | Sets the interrupt monitor. |
| [SetRibbonXml(const U16String\& value)](./setribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
| [SetRibbonXml(const char16_t* value)](./setribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
| [SetThemeColor(ThemeColorType type, const Aspose::Cells::Color\& color)](./setthemecolor/) | Sets the theme color. |
| [StartAccessCache(AccessCacheOptions opts)](./startaccesscache/) | Starts the session that uses caches to access data. |
| [Unprotect(const U16String\& password)](./unprotect/) | Unprotects a workbook. |
| [Unprotect(const char16_t* password)](./unprotect/) | Unprotects a workbook. |
| [UnprotectSharedWorkbook(const U16String\& password)](./unprotectsharedworkbook/) | Unprotects a shared workbook. |
| [UnprotectSharedWorkbook(const char16_t* password)](./unprotectsharedworkbook/) | Unprotects a shared workbook. |
| [UpdateCustomFunctionDefinition(CustomFunctionDefinition* definition)](./updatecustomfunctiondefinition/) | Updates definition of custom functions. |
| [UpdateLinkedDataSource(const Vector \<Workbook\>\& externalWorkbooks)](./updatelinkeddatasource/) | If this workbook contains external links to other data source, [Aspose.Cells](../) will attempt to retrieve the latest data from give sources. |
| [Workbook()](./workbook/) | Initializes a new instance of the [Workbook](./) class. |
| explicit [Workbook(FileFormatType fileFormatType)](./workbook/) | Initializes a new instance of the [Workbook](./) class. |
| explicit [Workbook(const U16String\& file)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open a file. |
| explicit [Workbook(const char16_t* file)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open a file. |
| explicit [Workbook(const Vector \<uint8_t\>\& stream)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open a stream. |
| [Workbook(const U16String\& file, const LoadOptions\& loadOptions)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open a file. |
| [Workbook(const char16_t* file, const LoadOptions\& loadOptions)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open a file. |
| [Workbook(const Vector \<uint8_t\>\& stream, const LoadOptions\& loadOptions)](./workbook/) | Initializes a new instance of the [Workbook](./) class and open stream. |
| [Workbook(Workbook_Impl* impl)](./workbook/) | Constructs from an implementation object. |
| [Workbook(const Workbook\& src)](./workbook/) | Copy constructor. |
| [~Workbook()](./~workbook/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
The [Workbook](./) class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks, converting Excel to PDF, rendering Excel to image and protecting the Excel spreadsheet.
## Examples
```cpp
Aspose::Cells::Startup();
//Open a designer file
U16String designerFile = u"designer.xls";
Workbook workbook(designerFile);
//Set scroll bars
workbook.GetSettings().SetIsHScrollBarVisible(false);
workbook.GetSettings().SetIsVScrollBarVisible(false);
//Replace the placeholder string with new values
int newInt = 100;
workbook.Replace(u"OldInt", newInt);
U16String oldString = u"Hi!";
U16String newString = u"Hello!";
workbook.Replace(oldString, newString);
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
