##Aspose::Cells::WorksheetCollection class
'Aspose::Cells::WorksheetCollection class. Encapsulates a collection of Worksheet objects in C++.'
## WorksheetCollection class
Encapsulates a collection of [Worksheet](../worksheet/) objects.
```cpp
class WorksheetCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(SheetType type)](./add/) | Adds a worksheet to the collection. |
| [Add()](./add/) | Adds a worksheet to the collection. |
| [Add(const U16String\& sheetName)](./add/) | Adds a worksheet to the collection. |
| [Add(const char16_t* sheetName)](./add/) | Adds a worksheet to the collection. |
| [AddCopy(const U16String\& sheetName)](./addcopy/) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy(const char16_t* sheetName)](./addcopy/) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy(int32_t sheetIndex)](./addcopy/) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy(const Vector \<Worksheet\>\& source, const Vector \<U16String\>\& destSheetNames)](./addcopy/) | Copy a group of worksheets. |
| [Clear()](./clear/) | Clear all worksheets. |
| [ClearPivottables()](./clearpivottables/) | Clears pivot tables from the spreadsheet. |
| [CreateRange(const U16String\& address, int32_t sheetIndex)](./createrange/) | Creates a [Range](../range/) object from an address of the range. |
| [CreateRange(const char16_t* address, int32_t sheetIndex)](./createrange/) | Creates a [Range](../range/) object from an address of the range. |
| [CreateUnionRange(const U16String\& address, int32_t sheetIndex)](./createunionrange/) | Creates a [Range](../range/) object from an address of the range. |
| [CreateUnionRange(const char16_t* address, int32_t sheetIndex)](./createunionrange/) | Creates a [Range](../range/) object from an address of the range. |
| [Get(int32_t index)](./get/) | Gets the [Worksheet](../worksheet/) element at the specified index. |
| [Get(const U16String\& sheetName)](./get/) | Gets the [Worksheet](../worksheet/) element with the specified name. |
| [Get(const char16_t* sheetName)](./get/) | Gets the [Worksheet](../worksheet/) element with the specified name. |
| [GetActiveSheetIndex()](./getactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. |
| [GetActiveSheetName()](./getactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. |
| [GetBuiltInDocumentProperties()](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
| [GetCount()](./getcount/) |  |
| [GetCustomDocumentProperties()](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [GetDxfs()](./getdxfs/) | Gets the master differential formatting records. |
| [GetExternalLinks()](./getexternallinks/) | Represents external links in a workbook. |
| [GetNamedRanges()](./getnamedranges/) | Gets all pre-defined named ranges in the spreadsheet. |
| [GetNamedRangesAndTables()](./getnamedrangesandtables/) | Gets all pre-defined named ranges in the spreadsheet. |
| [GetNames()](./getnames/) | Gets the collection of all the [Name](../name/) objects in the spreadsheet. |
| [GetOleSize()](./getolesize/) | Gets and Sets displayed size when [Workbook](../workbook/) file is used as an Ole object. |
| [GetRangeByName(const U16String\& rangeName)](./getrangebyname/) | Gets [Range](../range/) object by pre-defined name. |
| [GetRangeByName(const char16_t* rangeName)](./getrangebyname/) | Gets [Range](../range/) object by pre-defined name. |
| [GetRangeByName(const U16String\& rangeName, int32_t currentSheetIndex, bool includeTable)](./getrangebyname/) | Gets [Range](../range/) by pre-defined name or table's name. |
| [GetRangeByName(const char16_t* rangeName, int32_t currentSheetIndex, bool includeTable)](./getrangebyname/) | Gets [Range](../range/) by pre-defined name or table's name. |
| [GetRevisionLogs()](./getrevisionlogs/) | Represents revision logs. |
| [GetSensitivityLabels()](./getsensitivitylabels/) | Represents all sensitivity labels. |
| [GetSheetByCodeName(const U16String\& codeName)](./getsheetbycodename/) | Gets the worksheet by the code name. |
| [GetSheetByCodeName(const char16_t* codeName)](./getsheetbycodename/) | Gets the worksheet by the code name. |
| [GetTableStyles()](./gettablestyles/) | Gets TableStyles object. |
| [GetThreadedCommentAuthors()](./getthreadedcommentauthors/) | Gets the list of threaded comment authors. |
| [GetWebExtensions()](./getwebextensions/) | Gets the list of task panes. |
| [GetWebExtensionTaskPanes()](./getwebextensiontaskpanes/) | Gets the list of task panes. |
| [GetXmlMaps()](./getxmlmaps/) | Gets and sets the XML maps in the workbook. |
| [Insert(int32_t index, SheetType sheetType)](./insert/) | Insert a worksheet. |
| [Insert(int32_t index, SheetType sheetType, const U16String\& sheetName)](./insert/) | Insert a worksheet. |
| [Insert(int32_t index, SheetType sheetType, const char16_t* sheetName)](./insert/) | Insert a worksheet. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRefreshAllConnections()](./isrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WorksheetCollection\& src)](./operator_asm/) | operator= |
| [RefreshAll()](./refreshall/) | Refresh all pivot tables and charts with pivot source. |
| [RefreshPivotTables()](./refreshpivottables/) | Refreshes all the PivotTables in the Excel file. |
| [RefreshPivotTables(const PivotTableRefreshOption\& option)](./refreshpivottables/) | Refreshes all the PivotTables in the Excel file. |
| [RegisterAddInFunction(const U16String\& addInFile, const U16String\& functionName, bool lib)](./registeraddinfunction/) | Adds addin function into the workbook. |
| [RegisterAddInFunction(const char16_t* addInFile, const char16_t* functionName, bool lib)](./registeraddinfunction/) | Adds addin function into the workbook. |
| [RegisterAddInFunction(int32_t id, const U16String\& functionName)](./registeraddinfunction/) | Adds addin function into the workbook. |
| [RegisterAddInFunction(int32_t id, const char16_t* functionName)](./registeraddinfunction/) | Adds addin function into the workbook. |
| [RemoveAt(const U16String\& name)](./removeat/) | Removes the element at a specified name. |
| [RemoveAt(const char16_t* name)](./removeat/) | Removes the element at a specified name. |
| [RemoveAt(int32_t index)](./removeat/) | Removes the element at a specified index. |
| [SetActiveSheetIndex(int32_t value)](./setactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. |
| [SetActiveSheetName(const U16String\& value)](./setactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. |
| [SetActiveSheetName(const char16_t* value)](./setactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. |
| [SetIsRefreshAllConnections(bool value)](./setisrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. |
| [SetOleSize(const Aspose::Cells::Object\& value)](./setolesize/) | Gets and Sets displayed size when [Workbook](../workbook/) file is used as an Ole object. |
| [SetOleSize(int32_t startRow, int32_t endRow, int32_t startColumn, int32_t endColumn)](./setolesize/) | Sets displayed size when [Workbook](../workbook/) file is used as an Ole object. |
| [SetXmlMaps(const XmlMapCollection\& value)](./setxmlmaps/) | Gets and sets the XML maps in the workbook. |
| [SortNames()](./sortnames/) | Sorts the defined names. |
| [SwapSheet(int32_t sheetIndex1, int32_t sheetIndex2)](./swapsheet/) | Swaps the two sheets. |
| [WorksheetCollection(WorksheetCollection_Impl* impl)](./worksheetcollection/) | Constructs from an implementation object. |
| [WorksheetCollection(const WorksheetCollection\& src)](./worksheetcollection/) | Copy constructor. |
| [~WorksheetCollection()](./~worksheetcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
WorksheetCollection sheets = workbook.GetWorksheets();
//Add a worksheet
sheets.Add();
//Change the name of a worksheet
sheets.Get(0).SetName(u"First Sheet");
//Set the active sheet to the second worksheet
sheets.SetActiveSheetIndex(1);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
