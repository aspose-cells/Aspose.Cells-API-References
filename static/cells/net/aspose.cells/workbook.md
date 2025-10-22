##Class Workbook
Aspose.Cells.Workbook class. Represents a root object to create an Excel spreadsheet
## Workbook class
Represents a root object to create an Excel spreadsheet.
```csharp
public class Workbook : IDisposable
```
## Constructors
| Name | Description |
| --- | --- |
| [Workbook](workbook/#constructor)() | Initializes a new instance of the `Workbook` class. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Initializes a new instance of the `Workbook` class. |
| [Workbook](workbook/#constructor_2)(Stream) | Initializes a new instance of the `Workbook` class and open a stream. |
| [Workbook](workbook/#constructor_4)(string) | Initializes a new instance of the `Workbook` class and open a file. |
| [Workbook](workbook/#constructor_3)(Stream, LoadOptions) | Initializes a new instance of the `Workbook` class and open stream. |
| [Workbook](workbook/#constructor_5)(string, LoadOptions) | Initializes a new instance of the `Workbook` class and open a file. |
## Properties
| Name | Description |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Gets and sets the absolute path of the file. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Gets the factory for building ICellsDataTable from custom objects |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Returns colors in the palette for the spreadsheet. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Gets the list of [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) objects in the workbook. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Gets number of the styles in the style pool. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Gets the [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/) collection. |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Gets mashup data. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Gets data model in the workbook. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Gets a DataSorter object to sort data. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Gets or sets the default [`Style`](../style/) object of the workbook. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Gets and sets the file format. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Gets and sets the current file name. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Detects whether there is custom function used in this workbook, such as in cell's formula, in defined names... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Indicates if this spreadsheet contains macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Gets if the workbook has any tracked changes |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Gets and sets the interrupt monitor. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Indicates if this spreadsheet is digitally signed. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Indicates whether license is set. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Indicates whether structure or window is protected with password. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Gets and sets the XML file that defines the Ribbon UI. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Represents the workbook settings. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Gets the theme name. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Gets the [`VbaProject`](./vbaproject/) in a spreadsheet. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Gets the [`WorksheetCollection`](../worksheetcollection/) collection in the spreadsheet. |
## Methods
| Name | Description |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Accepts all tracked changes in the workbook. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Calculates the result of formulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Calculates the result of formulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Calculating formulas in this workbook. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Changes the palette for the spreadsheet in the specified index. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Closes the session that uses caches to access data. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Combines another Workbook object. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Copies data from a source Workbook object. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Copies another Workbook object. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Copies the theme from another workbook. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Creates built-in style by given type. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Creates a [`CellsColor`](../cellscolor/) object. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Creates a new style. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Creates a new style. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Customs the theme. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Export XML data. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Export XML data linked by the specified XML map. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Gets digital signature from file. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Gets all fonts in the style pool. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Find best matching Color in current palette. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Gets the named style in the style pool. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Gets theme color. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Indicates whether this workbook contains external links to other data sources. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Imports/Updates an XML data file into the workbook. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Imports/Updates an XML data file into the workbook. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Checks if a color is in the palette for the spreadsheet. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Merges named styles from the other Excel file. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Protects a workbook. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Protects a shared workbook. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Removes digital signature from this spreadsheet. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Removes all external links in the workbook. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Removes VBA/macro from this spreadsheet. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Removes personal information. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Remove all unused styles. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Replaces cells' values with new data. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Replaces cells' values with new data. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Replaces cells' values with data from a DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Replaces a cell's value with a new double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Replaces a cell's value with a new integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Replaces a cell's value with a new string. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Replaces cells' values with a double array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Replaces cells' values with an integer array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Replaces a cell's value with a new string. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Replaces a cell's value with a new string array. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Save the workbook to the disk. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Saves the workbook to the stream. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Saves the workbook to the stream. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Saves the workbook to the disk. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Saves the workbook to the disk. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Saves Excel file to a MemoryStream object as an Excel97-2003 xls file and returns it. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Set Encryption Options. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Sets the theme color |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Starts the session that uses caches to access data. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Unprotects a workbook. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Unprotects a shared workbook. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Updates definition of custom functions. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources. |
### Remarks
The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks, converting Excel to PDF, rendering Excel to image and protecting the Excel spreadsheet.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorkbookDemo
{
public static void WorkbookExample()
{
// Create a new Workbook instance
Workbook workbook = new Workbook();
// Access the default worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some properties of the workbook
workbook.FileName = "ExampleWorkbook.xlsx";
workbook.DefaultStyle.Font.Name = "Tahoma";
// Add a new worksheet
int newSheetIndex = workbook.Worksheets.Add();
Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
newWorksheet.Name = "NewSheet";
// Add some data to the new worksheet
newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
// Set some document properties
workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
workbook.CustomDocumentProperties.Add("Checked by", "Jane");
// Save the workbook to a file
workbook.Save("WorkbookExample.xlsx");
// Display some properties
Console.WriteLine("Workbook File Name: " + workbook.FileName);
Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);
// Check if the workbook is licensed
Console.WriteLine("Is Licensed: " + workbook.IsLicensed);
// Check if the workbook is digitally signed
Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);
// Check if the workbook contains macros
Console.WriteLine("Has Macros: " + workbook.HasMacro);
// Check if the workbook has any tracked changes
Console.WriteLine("Has Revisions: " + workbook.HasRevisions);
// Check the number of styles in the style pool
Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);
// Check the theme name
Console.WriteLine("Theme: " + workbook.Theme);
// Check if the workbook is protected with a password
Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);
// Check if the workbook contains external links
Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));
// Dispose the workbook
workbook.Dispose();
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
