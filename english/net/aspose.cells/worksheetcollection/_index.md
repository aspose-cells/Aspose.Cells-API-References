---
title: WorksheetCollection
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates a collection of Worksheet./worksheet objects.
type: docs
weight: 6550
url: /net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Encapsulates a collection of [`Worksheet`](../worksheet) objects.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Properties

| Name | Description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Represents the index of active worksheet when the spreadsheet is opened. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Represents the name of active worksheet when the spreadsheet is opened. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Gets the master differential formatting records. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Represents external links in a workbook. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Indicates whether refresh all connections on opening file in MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Gets the [`Worksheet`](../worksheet) element at the specified index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Gets the collection of all the Name objects in the spreadsheet. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Represents revision logs. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Gets [`TableStyles`](./tablestyles) object. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Gets the list of threaded comment authors. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Gets the list of task panes. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Gets the list of task panes. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Gets and sets the XML maps in the workbook. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Adds a worksheet to the collection. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Adds a worksheet to the collection. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Adds a worksheet to the collection. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Clear all worksheets. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Clears pivot tables from the spreadsheet. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Creates a [`Range`](../range) object from an address of the range. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Creates a [`Range`](../range) object from an address of the range. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Gets all pre-defined named ranges in the spreadsheet. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Gets all pre-defined named ranges in the spreadsheet. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Gets Range object by pre-defined name. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Gets [`Range`](../range) by pre-defined name or table's name |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Gets the worksheet by the code name. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Insert a worksheet. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Insert a worksheet. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Refreshes all the PivotTables in the WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Adds addin function into the workbook |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Adds addin function into the workbook |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Removes the element at a specified index. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Removes the element at a specified name. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Sets displayed size when Workbook file is used as an Ole object. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Sorts the defined names. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Swaps the two sheets. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Add a worksheet
sheets.Add();

//Change the name of a worksheet
sheets[0].Name = "First Sheet";

//Set the active sheet to the second worksheet
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Add a worksheet
sheets.Add()

'Change the name of a worksheet
sheets(0).Name = "First Sheet"

'Set the active sheet to the second worksheet
sheets.ActiveSheetIndex = 1
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
