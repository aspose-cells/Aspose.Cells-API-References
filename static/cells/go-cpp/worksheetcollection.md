##WorksheetCollection Class
'WorksheetCollection class. Encapsulates the object that represents worksheetcollection in Go.'
## WorksheetCollection class
Encapsulates a collection of <see cref="Worksheet"/> objects.
```go
type WorksheetCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Gets the list of task panes. |
|[GetWebExtensions](./getwebextensions/) | Gets the list of task panes. |
|[GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Gets the list of threaded comment authors. |
|[IsRefreshAllConnections](./isrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. |
|[SetIsRefreshAllConnections](./setisrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. |
|[CreateRange](./createrange/) | Creates a Range object from an address of the range. |
|[CreateUnionRange](./createunionrange/) | Creates a Range object from an address of the range. |
|[GetNames](./getnames/) | Gets the collection of all the Name objects in the spreadsheet. |
|[Get_Int](./get_int/) | Gets the Worksheet element at the specified index. |
|[Get_String](./get_string/) | Gets the Worksheet element with the specified name. |
|[GetSheetByCodeName](./getsheetbycodename/) | Gets the worksheet by the code name. |
|[GetActiveSheetName](./getactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. |
|[SetActiveSheetName](./setactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. |
|[GetActiveSheetIndex](./getactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. |
|[SetActiveSheetIndex](./setactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. |
|[SortNames](./sortnames/) | Sorts the defined names. |
|[Insert_Int_SheetType](./insert_int_sheettype/) | Insert a worksheet. |
|[Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Insert a worksheet. |
|[Add_SheetType](./add_sheettype/) | Adds a worksheet to the collection. |
|[SwapSheet](./swapsheet/) | Swaps the two sheets. |
|[Add](./add/) | Adds a worksheet to the collection. |
|[Add_String](./add_string/) | Adds a worksheet to the collection. |
|[RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Adds addin function into the workbook |
|[RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Adds addin function into the workbook |
|[RemoveAt_String](./removeat_string/) | Removes the element at a specified name. |
|[RemoveAt_Int](./removeat_int/) | Removes the element at a specified index. |
|[Clear](./clear/) | Clear all worksheets. |
|[AddCopy_String](./addcopy_string/) | Adds a worksheet to the collection and copies data from an existed worksheet. |
|[AddCopy_Int](./addcopy_int/) | Adds a worksheet to the collection and copies data from an existed worksheet. |
|[AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Copy a group of worksheets. |
|[GetDxfs](./getdxfs/) | Gets the master differential formatting records. |
|[GetRangeByName_String](./getrangebyname_string/) | Gets Range object by pre-defined name. |
|[GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Gets Range by pre-defined name or table's name |
|[GetNamedRanges](./getnamedranges/) | Gets all pre-defined named ranges in the spreadsheet. |
|[GetNamedRangesAndTables](./getnamedrangesandtables/) | Gets all pre-defined named ranges in the spreadsheet. |
|[GetXmlMaps](./getxmlmaps/) | Gets and sets the XML maps in the workbook. |
|[SetXmlMaps](./setxmlmaps/) | Gets and sets the XML maps in the workbook. |
|[GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
|[GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
|[GetOleSize](./getolesize/) | Gets and Sets displayed size when Workbook file is used as an Ole object. |
|[SetOleSize_Object](./setolesize_object/) | Gets and Sets displayed size when Workbook file is used as an Ole object. |
|[SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Sets displayed size when Workbook file is used as an Ole object. |
|[GetExternalLinks](./getexternallinks/) | Represents external links in a workbook. |
|[GetTableStyles](./gettablestyles/) | Gets TableStyles object. |
|[ClearPivottables](./clearpivottables/) | Clears pivot tables from the spreadsheet. |
|[GetRevisionLogs](./getrevisionlogs/) | Represents revision logs. |
|[RefreshAll](./refreshall/) | Refresh all pivot tables and charts with pivot source. |
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in the Excel file. |
|[RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Refreshes all the PivotTables in the Excel file. |
|[GetSensitivityLabels](./getsensitivitylabels/) | Represents all sensitivity labels. |
|[GetCount](./getcount/) |  |
