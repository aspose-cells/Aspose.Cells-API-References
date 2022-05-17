---
title: Workbook
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 6470
url: /net/aspose.cells/workbook/
---
## Workbook class

Represents a root object to create an Excel spreadsheet.

```csharp
public class Workbook : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [Workbook](workbook)() | Initializes a new instance of the [`Workbook`](../workbook) class. |
| [Workbook](workbook)(FileFormatType) | Initializes a new instance of the [`Workbook`](../workbook) class. |
| [Workbook](workbook)(Stream) | Initializes a new instance of the [`Workbook`](../workbook) class and open a stream. |
| [Workbook](workbook)(string) | Initializes a new instance of the [`Workbook`](../workbook) class and open a file. |
| [Workbook](workbook)(Stream, LoadOptions) | Initializes a new instance of the [`Workbook`](../workbook) class and open stream. |
| [Workbook](workbook)(string, LoadOptions) | Initializes a new instance of the [`Workbook`](../workbook) class and open a file. |

## Properties

| Name | Description |
| --- | --- |
| [AbsolutePath](absolutepath) { get; set; } | Gets and sets the absolute path of the file. |
| [BuiltInDocumentProperties](builtindocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [Colors](colors) { get; } | Returns colors in the palette for the spreadsheet. |
| [ContentTypeProperties](contenttypeproperties) { get; } | Gets the list of [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) objects in the workbook. |
| [CountOfStylesInPool](countofstylesinpool) { get; } | Gets number of the styles in the style pool. |
| [CustomDocumentProperties](customdocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [CustomXmlParts](customxmlparts) { get; } | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [DataConnections](dataconnections) { get; } | Gets the [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) collection. |
| [DataMashup](datamashup) { get; } | Gets mashup data. |
| [DataSorter](datasorter) { get; } | Gets a DataSorter object to sort data. |
| [DefaultStyle](defaultstyle) { get; set; } | Gets or sets the default [`Style`](../style) object of the workbook. |
| [FileFormat](fileformat) { get; set; } | Gets and sets the file format. |
| [FileName](filename) { get; set; } | Gets and sets the current file name. |
| [HasMacro](hasmacro) { get; } | Indicates if this spreadsheet contains macro/VBA. |
| [HasRevisions](hasrevisions) { get; } | Gets if the workbook has any tracked changes |
| [InterruptMonitor](interruptmonitor) { get; set; } | Gets and sets the interrupt monitor. |
| [IsDigitallySigned](isdigitallysigned) { get; } | Indicates if this spreadsheet is digitally signed. |
| [IsLicensed](islicensed) { get; } | Indicates whether license is set. |
| [IsWorkbookProtectedWithPassword](isworkbookprotectedwithpassword) { get; } | Indicates whether structure or window is protected with password. |
| [RibbonXml](ribbonxml) { get; set; } | Gets and sets the XML file that defines the Ribbon UI. |
| [Settings](settings) { get; } | Represents the workbook settings. |
| [Theme](theme) { get; } | Gets the theme name. |
| [VbaProject](vbaproject) { get; } | Gets the [`VbaProject`](./vbaproject) in a spreadsheet. |
| [Worksheets](worksheets) { get; } | Gets the [`WorksheetCollection`](../worksheetcollection) collection in the spreadsheet. |

## Methods

| Name | Description |
| --- | --- |
| [AcceptAllRevisions](acceptallrevisions)() | Accepts all tracked changes in the workbook. |
| [AddDigitalSignature](adddigitalsignature)(DigitalSignatureCollection) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [CalculateFormula](calculateformula)() | Calculates the result of formulas. |
| [CalculateFormula](calculateformula)(bool) | Calculates the result of formulas. |
| [CalculateFormula](calculateformula)(CalculationOptions) | Calculating formulas in this workbook. |
| [ChangePalette](changepalette)(Color, int) | Changes the palette for the spreadsheet in the specified index. |
| [CloseAccessCache](closeaccesscache)(AccessCacheOptions) | Closes the session that uses caches to access data. |
| [Combine](combine)(Workbook) | Combines another Workbook object. |
| [Copy](copy)(Workbook) | Copies data from a source Workbook object. |
| [Copy](copy)(Workbook, CopyOptions) | Copies data from a source Workbook object. |
| [CopyTheme](copytheme)(Workbook) | Copies the theme from another workbook. |
| [CreateBuiltinStyle](createbuiltinstyle)(BuiltinStyleType) | Creates built-in style by given type. |
| [CreateCellsColor](createcellscolor)() | Creates a [`CellsColor`](../cellscolor) object. |
| [CreateStyle](createstyle)() | Creates a new style. |
| [CustomTheme](customtheme)(string, Color[]) | Customs the theme. |
| [Dispose](dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExportXml](exportxml)(string, Stream) | Export XML data. |
| [ExportXml](exportxml)(string, string) | Export XML data linked by the specified XML map. |
| [GetDigitalSignature](getdigitalsignature)() | Gets digital signature from file. |
| [GetFonts](getfonts)() | Gets all fonts in the style pool. |
| [GetMatchingColor](getmatchingcolor)(Color) | Find best matching Color in current palette. |
| [GetNamedStyle](getnamedstyle)(string) | Gets the named style in the style pool. |
| [GetStyleInPool](getstyleinpool)(int) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. |
| [GetThemeColor](getthemecolor)(ThemeColorType) | Gets theme color. |
| [ImportXml](importxml)(Stream, string, int, int) | Imports/Updates an XML data file into the workbook. |
| [ImportXml](importxml)(string, string, int, int) | Imports/Updates an XML data file into the workbook. |
| [IsColorInPalette](iscolorinpalette)(Color) | Checks if a color is in the palette for the spreadsheet. |
| [ParseFormulas](parseformulas)(bool) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [Protect](protect)(ProtectionType, string) | Protects a workbook. |
| [ProtectSharedWorkbook](protectsharedworkbook)(string) | Protects a shared workbook. |
| [RefreshDynamicArrayFormulas](refreshdynamicarrayformulas)(bool) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [RemoveDigitalSignature](removedigitalsignature)() | Removes digital signature from this spreadsheet. |
| [RemoveMacro](removemacro)() | Removes VBA/macro from this spreadsheet. |
| [RemovePersonalInformation](removepersonalinformation)() | Removes personal information. |
| [RemoveUnusedStyles](removeunusedstyles)() | Remove all unused styles. |
| [Replace](replace)(bool, object) | Replaces cells' values with new data. |
| [Replace](replace)(int, object) | Replaces cells' values with new data. |
| [Replace](replace)(string, DataTable) | Replaces cells' values with data from a DataTable. |
| [Replace](replace)(string, double) | Replaces a cell's value with a new double. |
| [Replace](replace)(string, int) | Replaces a cell's value with a new integer. |
| [Replace](replace)(string, string) | Replaces a cell's value with a new string. |
| [Replace](replace)(string, double[], bool) | Replaces cells' values with a double array. |
| [Replace](replace)(string, int[], bool) | Replaces cells' values with an integer array. |
| [Replace](replace)(string, string, ReplaceOptions) | Replaces a cell's value with a new string. |
| [Replace](replace)(string, string[], bool) | Replaces a cell's value with a new string array. |
| [Save](save)(string) | Save the workbook to the disk. |
| [Save](save)(Stream, SaveFormat) | Saves the workbook to the stream. |
| [Save](save)(Stream, SaveOptions) | Saves the workbook to the stream. |
| [Save](save)(string, SaveFormat) | Saves the workbook to the disk. |
| [Save](save)(string, SaveOptions) | Saves the workbook to the disk. |
| [Save](save)(HttpResponse, string, ContentDisposition, SaveOptions) | Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook. |
| [Save](save)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook. |
| [SaveToStream](savetostream)() | Saves Excel file to a MemoryStream object and returns it. |
| [SetDigitalSignature](setdigitalsignature)(DigitalSignatureCollection) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [SetEncryptionOptions](setencryptionoptions)(EncryptionType, int) | Set Encryption Options. |
| [SetThemeColor](setthemecolor)(ThemeColorType, Color) | Sets the theme color |
| [StartAccessCache](startaccesscache)(AccessCacheOptions) | Starts the session that uses caches to access data. |
| [Unprotect](unprotect)(string) | Unprotects a workbook. |
| [UnprotectSharedWorkbook](unprotectsharedworkbook)(string) | Unprotects a shared workbook. |
| [UpdateLinkedDataSource](updatelinkeddatasource)(Workbook[]) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data. |

### Remarks

The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks and protecting the Excel spreadsheet.

### Examples

The following example loads a Workbook from a file named designer.xls and makes the horizontal and vertical scroll bars invisible for the Workbook. It then replaces two string values with an Integer value and string value respectively within the spreadsheet and finally sends the updated file to the client browser.

```csharp
[C#]

//Open a designer file
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Set scroll bars
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Replace the placeholder string with new values
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Open a designer file
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Set scroll bars
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Replace the placeholder string with new values
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
