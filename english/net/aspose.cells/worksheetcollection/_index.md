---
title: WorksheetCollection
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 6490
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
| [ActiveSheetIndex](activesheetindex) { get; set; } | Represents the index of active worksheet when the spreadsheet is opened. |
| [ActiveSheetName](activesheetname) { get; set; } | Represents the name of active worksheet when the spreadsheet is opened. |
| [BuiltInDocumentProperties](builtindocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [CustomDocumentProperties](customdocumentproperties) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [Dxfs](dxfs) { get; } | Gets the master differential formatting records. |
| [ExternalLinks](externallinks) { get; } | Represents external links in a workbook. |
| [IsRefreshAllConnections](isrefreshallconnections) { get; set; } | Indicates whether refresh all connections on opening file in MS Excel. |
| [Item](item) { get; } | Gets the [`Worksheet`](../worksheet) element at the specified index. (2 indexers) |
| [Names](names) { get; } | Gets the collection of all the Name objects in the spreadsheet. |
| [OleSize](olesize) { get; set; } | Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [RevisionLogs](revisionlogs) { get; } | Represents revision logs. |
| [TableStyles](tablestyles) { get; } | Gets [`TableStyles`](./tablestyles) object. |
| [ThreadedCommentAuthors](threadedcommentauthors) { get; } | Gets the list of threaded comment authors. |
| [WebExtensions](webextensions) { get; } | Gets the list of task panes. |
| [WebExtensionTaskPanes](webextensiontaskpanes) { get; } | Gets the list of task panes. |
| [XmlMaps](xmlmaps) { get; set; } | Gets and sets the XML maps in the workbook. |

## Methods

| Name | Description |
| --- | --- |
| [Add](add)() | Adds a worksheet to the collection. |
| [Add](add)(SheetType) | Adds a worksheet to the collection. |
| [Add](add)(string) | Adds a worksheet to the collection. |
| [AddCopy](addcopy)(int) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [AddCopy](addcopy)(string) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [Clear](clear)() | Clear all worksheets. |
| [ClearPivottables](clearpivottables)() | Clears pivot tables from the spreadsheet. |
| [CreateRange](createrange)(string, int) | Creates a [`Range`](../range) object from an address of the range. |
| [CreateUnionRange](createunionrange)(string, int) | Creates a [`Range`](../range) object from an address of the range. |
| [GetNamedRanges](getnamedranges)() | Gets all pre-defined named ranges in the spreadsheet. |
| [GetNamedRangesAndTables](getnamedrangesandtables)() | Gets all pre-defined named ranges in the spreadsheet. |
| [GetRangeByName](getrangebyname)(string) | Gets Range object by pre-defined name. |
| [GetRangeByName](getrangebyname)(string, int, bool) | Gets [`Range`](../range) by pre-defined name or table's name |
| [GetSheetByCodeName](getsheetbycodename)(string) | Gets the worksheet by the code name. |
| [Insert](insert)(int, SheetType) | Insert a worksheet. |
| [Insert](insert)(int, SheetType, string) | Insert a worksheet. |
| [RefreshPivotTables](refreshpivottables)() | Refreshes all the PivotTables in the WorksheetCollection. |
| [RegisterAddInFunction](registeraddinfunction)(int, string) | Adds addin function into the workbook |
| [RegisterAddInFunction](registeraddinfunction)(string, string, bool) | Adds addin function into the workbook |
| [RemoveAt](removeat)(int) | Removes the element at a specified index. |
| [RemoveAt](removeat)(string) | Removes the element at a specified name. |
| [SetOleSize](setolesize)(int, int, int, int) | Sets displayed size when Workbook file is used as an Ole object. |
| [SortNames](sortnames)() | Sorts the defined names. |
| [SwapSheet](swapsheet)(int, int) | Swaps the two sheets. |

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
