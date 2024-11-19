---
title: Workbook Class 
linktitle: Workbook
second_title: Aspose.Cells for Go API Reference
description: 'Workbook class. Encapsulates the object that represents workbook in Go.'
type: docs
weight: 200
url: /go/aspose.cells/workbook/
---

## Workbook class

Represents a root object to create an Excel spreadsheet.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewWorkbook](./newworkbook/) | Initializes a new instance of the <see cref="Workbook"/> class. | 
|[NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Initializes a new instance of the <see cref="Workbook"/> class. | 
|[NewWorkbook_String](./newworkbook_string/) | Initializes a new instance of the <see cref="Workbook"/> class and open a file. | 
|[NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Initializes a new instance of the <see cref="Workbook"/> class and open a file. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetSettings](./getsettings/) | Represents the workbook settings. | 
|[ParseFormulas](./parseformulas/) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. | 
|[StartAccessCache](./startaccesscache/) | Starts the session that uses caches to access data. | 
|[CloseAccessCache](./closeaccesscache/) | Closes the session that uses caches to access data. | 
|[Save](./save/) | Saves the workbook to the disk. | 
|[Save](./save/) | Save the workbook to the disk. | 
|[Save](./save/) | Saves the workbook to the disk. | 
|[GetWorksheets](./getworksheets/) | Gets the <see cref="WorksheetCollection"/> collection in the spreadsheet. | 
|[IsLicensed](./islicensed/) | Indicates whether license is set. | 
|[RemoveUnusedStyles](./removeunusedstyles/) | Remove all unused styles. | 
|[CreateStyle](./createstyle/) | Creates a new style. | 
|[CreateBuiltinStyle](./createbuiltinstyle/) | Creates built-in style by given type. | 
|[CreateCellsColor](./createcellscolor/) | Creates a <see cref="CellsColor"/> object. | 
|[Replace](./replace/) | Replaces a cell's value with a new string. | 
|[Replace](./replace/) | Replaces a cell's value with a new integer. | 
|[Replace](./replace/) | Replaces a cell's value with a new double. | 
|[Replace](./replace/) | Replaces cells' values with new data. | 
|[Replace](./replace/) | Replaces cells' values with new data. | 
|[Replace](./replace/) | Replaces a cell's value with a new string. | 
|[Copy](./copy/) | Copies another Workbook object. | 
|[Copy](./copy/) | Copies data from a source Workbook object. | 
|[Combine](./combine/) | Combines another Workbook object. | 
|[GetStyleInPool](./getstyleinpool/) | Gets the style in the style pool.All styles in the workbook will be gathered into a pool.There is only a simple reference index in the cells. | 
|[GetCountOfStylesInPool](./getcountofstylesinpool/) | Gets number of the styles in the style pool. | 
|[GetNamedStyle](./getnamedstyle/) | Gets the named style in the style pool. | 
|[ChangePalette](./changepalette/) | Changes the palette for the spreadsheet in the specified index. | 
|[IsColorInPalette](./iscolorinpalette/) | Checks if a color is in the palette for the spreadsheet. | 
|[CalculateFormula](./calculateformula/) | Calculates the result of formulas. | 
|[CalculateFormula](./calculateformula/) | Calculates the result of formulas. | 
|[CalculateFormula](./calculateformula/) | Calculating formulas in this workbook. | 
|[RefreshDynamicArrayFormulas](./refreshdynamicarrayformulas/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. | 
|[RefreshDynamicArrayFormulas](./refreshdynamicarrayformulas/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) | 
|[GetDefaultStyle](./getdefaultstyle/) | Gets or sets the default <see cref="Style"/> object of the workbook. | 
|[SetDefaultStyle](./setdefaultstyle/) | Gets or sets the default <see cref="Style"/> object of the workbook. | 
|[GetMatchingColor](./getmatchingcolor/) | Find best matching Color in current palette. | 
|[IsDigitallySigned](./isdigitallysigned/) | Indicates if this spreadsheet is digitally signed. | 
|[SetEncryptionOptions](./setencryptionoptions/) | Set Encryption Options. | 
|[Protect](./protect/) | Protects a workbook. | 
|[ProtectSharedWorkbook](./protectsharedworkbook/) | Protects a shared workbook. | 
|[Unprotect](./unprotect/) | Unprotects a workbook. | 
|[UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Unprotects a shared workbook. | 
|[IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Indicates whether structure or window is protected with password. | 
|[RemoveMacro](./removemacro/) | Removes VBA/macro from this spreadsheet. | 
|[GetVbaProject](./getvbaproject/) | Gets the <see cref="VbaProject"/> in a spreadsheet. | 
|[RemoveDigitalSignature](./removedigitalsignature/) | Removes digital signature from this spreadsheet. | 
|[AcceptAllRevisions](./acceptallrevisions/) | Accepts all tracked changes in the workbook. | 
|[GetHasMacro](./gethasmacro/) | Indicates if this spreadsheet contains macro/VBA. | 
|[GetHasRevisions](./gethasrevisions/) | Gets if the workbook has any tracked changes | 
|[GetFileName](./getfilename/) | Gets and sets the current file name. | 
|[SetFileName](./setfilename/) | Gets and sets the current file name. | 
|[GetDataSorter](./getdatasorter/) | Gets a DataSorter object to sort data. | 
|[GetThemeColor](./getthemecolor/) | Gets theme color. | 
|[SetThemeColor](./setthemecolor/) | Sets the theme color | 
|[GetTheme](./gettheme/) | Gets the theme name. | 
|[CopyTheme](./copytheme/) | Copies the theme from another workbook. | 
|[UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Updates definition of custom functions. | 
|[GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a <see cref="DocumentProperty"/> collection that represents all the built-in document properties of the spreadsheet. | 
|[GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a <see cref="DocumentProperty"/> collection that represents all the custom document properties of the spreadsheet. | 
|[GetFileFormat](./getfileformat/) | Gets and sets the file format. | 
|[SetFileFormat](./setfileformat/) | Gets and sets the file format. | 
|[GetInterruptMonitor](./getinterruptmonitor/) | Gets and sets the interrupt monitor. | 
|[SetInterruptMonitor](./setinterruptmonitor/) | Gets and sets the interrupt monitor. | 
|[SetInterruptMonitor](./setinterruptmonitor/) | Sets the interrupt monitor. | 
|[GetContentTypeProperties](./getcontenttypeproperties/) | Gets the list of  <see cref="ContentTypeProperty"/> objects in the workbook. | 
|[GetCustomXmlParts](./getcustomxmlparts/) | Represents a Custom XML Data Storage Part (custom XML data within a package). | 
|[GetDataMashup](./getdatamashup/) | Gets mashup data. | 
|[GetRibbonXml](./getribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. | 
|[SetRibbonXml](./setribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. | 
|[GetAbsolutePath](./getabsolutepath/) | Gets and sets the absolute path of the file. | 
|[SetAbsolutePath](./setabsolutepath/) | Gets and sets the absolute path of the file. | 
|[GetDataConnections](./getdataconnections/) | Gets the <see cref="ExternalConnection"/> collection. | 
|[ImportXml](./importxml/) | Imports/Updates an XML data file into the workbook. | 
|[ExportXml](./exportxml/) | Export XML data linked by the specified XML map. | 
|[SetDigitalSignature](./setdigitalsignature/) | Sets digital signature to an spreadsheet file (Excel2007 and later). | 
|[AddDigitalSignature](./adddigitalsignature/) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). | 
|[GetDigitalSignature](./getdigitalsignature/) | Gets digital signature from file. | 
|[RemovePersonalInformation](./removepersonalinformation/) | Removes personal information. | 
|[GetDataModel](./getdatamodel/) | Gets data model in the workbook. | 
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. | 
