---
title: Range
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates the object that represents a range of cells within a spreadsheet.
type: docs
weight: 5060
url: /net/aspose.cells/range/
---
## Range class

Encapsulates the object that represents a range of cells within a spreadsheet.

```csharp
public class Range
```

## Properties

| Name | Description |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Gets address of the range. |
| [CellCount](../../aspose.cells/range/cellcount) { get; } | Gets all cell count in the range. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Gets the count of columns in the range. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Sets or gets the column width of this range |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Gets the index of the first column of the range. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Gets the index of the first row of the range. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Gets all hyperlink in the range. |
| [Item](../../aspose.cells/range/item) { get; } | Gets [`Cell`](../cell) object in this range. |
| [Name](../../aspose.cells/range/name) { get; set; } | Gets or sets the name of the range. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Gets the range's refers to. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Gets the count of rows in the range. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Sets or gets the height of rows in this range |
| [Value](../../aspose.cells/range/value) { get; set; } | Gets and sets the value of the range. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Gets the [`Worksheet`](./worksheet)object which contains this range. |

## Methods

| Name | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Applies formats for a whole range. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Automaticall fill the target range. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Automaticall fill the target range. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Copying the range with paste special options. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Copies cell data (including formulas) from a source range. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Copies style settings from a source range. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Copies cell value from a source range. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Exports data in this range to a DataTable object. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Exports data in this range to a DataTable object. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Exports data in this range to a DataTable object. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Gets [`Cell`](../cell) object or null in this range. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Gets the enumerator for cells in this Range. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Gets [`Range`](../range) range by offset. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Returns a [`Range`](../range) object that represents the rectangular intersection of two ranges. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Indicates whether the range is intersect. |
| [Merge](../../aspose.cells/range/merge)() | Combines a range of cells into a single cell. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Move the current range to the dest range. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Set inside borders of the range. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Sets outline border around a range of cells. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Sets out line borders around a range of cells. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Sets the style of the range. |
| override [ToString](../../aspose.cells/range/tostring)() | Returns a string represents the current Range object. |
| [Union](../../aspose.cells/range/union)(Range) | Returns the union of two ranges. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Unmerges merged cells of this range. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.Worksheets[0].Cells;
// Create a range (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Set value to the range.
range.Value = "Hello";
//Save the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Get the first Worksheet Cells.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Create a range (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Set value to the range.
range.Value = "Hello"
'Save the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
