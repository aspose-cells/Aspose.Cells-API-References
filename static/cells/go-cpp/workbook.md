##Workbook Class
'Workbook class. Encapsulates the object that represents workbook in Go.'
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
|[NewWorkbook](./newworkbook/) | Initializes a new instance of the Workbook class. |
|[NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Initializes a new instance of the Workbook class. |
|[NewWorkbook_String](./newworkbook_string/) | Initializes a new instance of the Workbook class and open a file. |
|[NewWorkbook_Stream](./newworkbook_stream/) | Initializes a new instance of the Workbook class and open a stream. |
|[NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Initializes a new instance of the Workbook class and open a file. |
|[NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Initializes a new instance of the Workbook class and open stream. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSettings](./getsettings/) | Represents the workbook settings. |
|[ParseFormulas](./parseformulas/) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
|[StartAccessCache](./startaccesscache/) | Starts the session that uses caches to access data. |
|[CloseAccessCache](./closeaccesscache/) | Closes the session that uses caches to access data. |
|[Save_String_SaveFormat](./save_string_saveformat/) | Saves the workbook to the disk. |
|[Save_String](./save_string/) | Save the workbook to the disk. |
|[Save_String_SaveOptions](./save_string_saveoptions/) | Saves the workbook to the disk. |
|[Save_SaveFormat](./save_saveformat/) | Saves the workbook to the stream. |
|[Save_SaveOptions](./save_saveoptions/) | Saves the workbook to the stream. |
|[SaveToStream](./savetostream/) | Saves Excel file to a MemoryStream object as an Excel97-2003 xls file and returns it. |
|[GetWorksheets](./getworksheets/) | Gets the WorksheetCollection collection in the spreadsheet. |
|[IsLicensed](./islicensed/) | Indicates whether license is set. |
|[RemoveUnusedStyles](./removeunusedstyles/) | Remove all unused styles. |
|[CreateStyle](./createstyle/) | Creates a new style. |
|[CreateStyle_Bool](./createstyle_bool/) | Creates a new style. |
|[CreateBuiltinStyle](./createbuiltinstyle/) | Creates built-in style by given type. |
|[CreateCellsColor](./createcellscolor/) | Creates a CellsColor object. |
|[Replace_String_String](./replace_string_string/) | Replaces a cell's value with a new string. |
|[Replace_String_Int](./replace_string_int/) | Replaces a cell's value with a new integer. |
|[Replace_String_Double](./replace_string_double/) | Replaces a cell's value with a new double. |
|[Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Replaces a cell's value with a new string array. |
|[Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Replaces cells' values with an integer array. |
|[Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Replaces cells' values with a double array. |
|[Replace_Bool_Object](./replace_bool_object/) | Replaces cells' values with new data. |
|[Replace_Int_Object](./replace_int_object/) | Replaces cells' values with new data. |
|[Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Replaces a cell's value with a new string. |
|[Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Copies another Workbook object. |
|[Copy_Workbook](./copy_workbook/) | Copies data from a source Workbook object. |
|[Combine](./combine/) | Combines another Workbook object. |
|[GetColors](./getcolors/) | Returns colors in the palette for the spreadsheet. |
|[GetStyleInPool](./getstyleinpool/) | Gets the style in the style pool.All styles in the workbook will be gathered into a pool.There is only a simple reference index in the cells. |
|[GetCountOfStylesInPool](./getcountofstylesinpool/) | Gets number of the styles in the style pool. |
|[GetFonts](./getfonts/) | Gets all fonts in the style pool. |
|[GetNamedStyle](./getnamedstyle/) | Gets the named style in the style pool. |
|[MergeNamedStyles](./mergenamedstyles/) | Merges named styles from the other Excel file. |
|[ChangePalette](./changepalette/) | Changes the palette for the spreadsheet in the specified index. |
|[IsColorInPalette](./iscolorinpalette/) | Checks if a color is in the palette for the spreadsheet. |
|[CalculateFormula](./calculateformula/) | Calculates the result of formulas. |
|[CalculateFormula_Bool](./calculateformula_bool/) | Calculates the result of formulas. |
|[CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Calculating formulas in this workbook. |
|[RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. |
|[RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
|[GetDefaultStyle](./getdefaultstyle/) | Gets or sets the default Style object of the workbook. |
|[SetDefaultStyle](./setdefaultstyle/) | Gets or sets the default Style object of the workbook. |
|[GetMatchingColor](./getmatchingcolor/) | Find best matching Color in current palette. |
|[IsDigitallySigned](./isdigitallysigned/) | Indicates if this spreadsheet is digitally signed. |
|[SetEncryptionOptions](./setencryptionoptions/) | Set Encryption Options. |
|[Protect](./protect/) | Protects a workbook. |
|[ProtectSharedWorkbook](./protectsharedworkbook/) | Protects a shared workbook. |
|[Unprotect](./unprotect/) | Unprotects a workbook. |
|[UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Unprotects a shared workbook. |
|[IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Indicates whether structure or window is protected with password. |
|[RemoveMacro](./removemacro/) | Removes VBA/macro from this spreadsheet. |
|[GetVbaProject](./getvbaproject/) | Gets the VbaProject in a spreadsheet. |
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
|[CustomTheme](./customtheme/) | Customs the theme. |
|[CopyTheme](./copytheme/) | Copies the theme from another workbook. |
|[UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Updates definition of custom functions. |
|[UpdateLinkedDataSource](./updatelinkeddatasource/) | If this workbook contains external links to other data source,Aspose.Cells will attempt to retrieve the latest data from give sources. |
|[GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
|[GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
|[GetFileFormat](./getfileformat/) | Gets and sets the file format. |
|[SetFileFormat](./setfileformat/) | Gets and sets the file format. |
|[GetHasCustomFunction](./gethascustomfunction/) | Detects whether there is custom function used in this workbook,such as in cell's formula, in defined names... |
|[GetInterruptMonitor](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
|[SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Gets and sets the interrupt monitor. |
|[SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Sets the interrupt monitor. |
|[GetContentTypeProperties](./getcontenttypeproperties/) | Gets the list of  ContentTypeProperty objects in the workbook. |
|[GetCustomXmlParts](./getcustomxmlparts/) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
|[GetDataMashup](./getdatamashup/) | Gets mashup data. |
|[GetRibbonXml](./getribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
|[SetRibbonXml](./setribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
|[GetAbsolutePath](./getabsolutepath/) | Gets and sets the absolute path of the file. |
|[SetAbsolutePath](./setabsolutepath/) | Gets and sets the absolute path of the file. |
|[GetDataConnections](./getdataconnections/) | Gets the ExternalConnection collection. |
|[ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Imports/Updates an XML data file into the workbook. |
|[ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Imports/Updates an XML data file into the workbook. |
|[ExportXml_String_String](./exportxml_string_string/) | Export XML data linked by the specified XML map. |
|[ExportXml_String](./exportxml_string/) | Export XML data. |
|[SetDigitalSignature](./setdigitalsignature/) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
|[AddDigitalSignature](./adddigitalsignature/) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
|[GetDigitalSignature](./getdigitalsignature/) | Gets digital signature from file. |
|[RemovePersonalInformation](./removepersonalinformation/) | Removes personal information. |
|[GetDataModel](./getdatamodel/) | Gets data model in the workbook. |
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. |
