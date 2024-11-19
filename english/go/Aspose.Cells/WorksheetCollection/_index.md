---
title: WorksheetCollection Class 
linktitle: WorksheetCollection
second_title: Aspose.Cells for Go API Reference
description: 'WorksheetCollection class. Encapsulates the object that represents worksheetcollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells/worksheetcollection/
---

## WorksheetCollection class

Encapsulates a collection of <see cref="Worksheet"/> objects.

```go

type WorksheetCollection struct 

worksheetcollection, _ := asposecells.NewWorksheetCollection()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewWorksheetCollection](./newworksheetcollection/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Gets the list of task panes. | 
|[GetWebExtensions](./getwebextensions/) | Gets the list of task panes. | 
|[GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Gets the list of threaded comment authors. | 
|[IsRefreshAllConnections](./isrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. | 
|[SetIsRefreshAllConnections](./setisrefreshallconnections/) | Indicates whether refresh all connections on opening file in MS Excel. | 
|[CreateRange](./createrange/) | Creates a <see cref="Range"/> object from an address of the range. | 
|[CreateUnionRange](./createunionrange/) | Creates a <see cref="Range"/> object from an address of the range. | 
|[GetNames](./getnames/) | Gets the collection of all the Name objects in the spreadsheet. | 
|[Get](./get/) | Gets the <see cref="Worksheet"/> element at the specified index. | 
|[Get](./get/) | Gets the <see cref="Worksheet"/> element with the specified name. | 
|[GetSheetByCodeName](./getsheetbycodename/) | Gets the worksheet by the code name. | 
|[GetActiveSheetName](./getactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. | 
|[SetActiveSheetName](./setactivesheetname/) | Represents the name of active worksheet when the spreadsheet is opened. | 
|[GetActiveSheetIndex](./getactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. | 
|[SetActiveSheetIndex](./setactivesheetindex/) | Represents the index of active worksheet when the spreadsheet is opened. | 
|[SortNames](./sortnames/) | Sorts the defined names. | 
|[Insert](./insert/) | Insert a worksheet. | 
|[Insert](./insert/) | Insert a worksheet. | 
|[Add](./add/) | Adds a worksheet to the collection. | 
|[SwapSheet](./swapsheet/) | Swaps the two sheets. | 
|[Add](./add/) | Adds a worksheet to the collection. | 
|[Add](./add/) | Adds a worksheet to the collection. | 
|[RegisterAddInFunction](./registeraddinfunction/) | Adds addin function into the workbook | 
|[RegisterAddInFunction](./registeraddinfunction/) | Adds addin function into the workbook | 
|[RemoveAt](./removeat/) | Removes the element at a specified name. | 
|[RemoveAt](./removeat/) | Removes the element at a specified index. | 
|[Clear](./clear/) | Clear all worksheets. | 
|[AddCopy](./addcopy/) | Adds a worksheet to the collection and copies data from an existed worksheet. | 
|[AddCopy](./addcopy/) | Adds a worksheet to the collection and copies data from an existed worksheet. | 
|[GetDxfs](./getdxfs/) | Gets the master differential formatting records. | 
|[GetRangeByName](./getrangebyname/) | Gets Range object by pre-defined name. | 
|[GetRangeByName](./getrangebyname/) | Gets <see cref="Range"/> by pre-defined name or table's name | 
|[GetXmlMaps](./getxmlmaps/) | Gets and sets the XML maps in the workbook. | 
|[SetXmlMaps](./setxmlmaps/) | Gets and sets the XML maps in the workbook. | 
|[GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a <see cref="DocumentProperty"/> collection that represents all the built-in document properties of the spreadsheet. | 
|[GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a <see cref="DocumentProperty"/> collection that represents all the custom document properties of the spreadsheet. | 
|[GetOleSize](./getolesize/) | Gets and Sets displayed size when Workbook file is used as an Ole object. | 
|[SetOleSize](./setolesize/) | Gets and Sets displayed size when Workbook file is used as an Ole object. | 
|[SetOleSize](./setolesize/) | Sets displayed size when Workbook file is used as an Ole object. | 
|[GetExternalLinks](./getexternallinks/) | Represents external links in a workbook. | 
|[GetTableStyles](./gettablestyles/) | Gets <see cref="TableStyles"/> object. | 
|[ClearPivottables](./clearpivottables/) | Clears pivot tables from the spreadsheet. | 
|[GetRevisionLogs](./getrevisionlogs/) | Represents revision logs. | 
|[RefreshAll](./refreshall/) | Refresh all pivot tables and charts with pivot source. | 
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in the Excel file. | 
|[RefreshPivotTables](./refreshpivottables/) | Refreshes all the PivotTables in the Excel file. | 
|[GetCount](./getcount/) |  | 
