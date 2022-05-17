---
title: Range
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 5020
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
| [Address](address) { get; } | Gets address of the range. |
| [ColumnCount](columncount) { get; } | Gets the count of columns in the range. |
| [ColumnWidth](columnwidth) { get; set; } | Sets or gets the column width of this range |
| [CurrentRegion](currentregion) { get; } | Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [EntireColumn](entirecolumn) { get; } | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [EntireRow](entirerow) { get; } | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [FirstColumn](firstcolumn) { get; } | Gets the index of the first column of the range. |
| [FirstRow](firstrow) { get; } | Gets the index of the first row of the range. |
| [Hyperlinks](hyperlinks) { get; } | Gets all hyperlink in the range. |
| [Item](item) { get; } | Gets [`Cell`](../cell) object in this range. |
| [Name](name) { get; set; } | Gets or sets the name of the range. |
| [RefersTo](refersto) { get; } | Gets the range's refers to. |
| [RowCount](rowcount) { get; } | Gets the count of rows in the range. |
| [RowHeight](rowheight) { get; set; } | Sets or gets the height of rows in this range |
| [Value](value) { get; set; } | Gets and sets the value of the range. |
| [Worksheet](worksheet) { get; } | Gets the [`Worksheet`](./worksheet)object which contains this range. |

## Methods

| Name | Description |
| --- | --- |
| [ApplyStyle](applystyle)(Style, StyleFlag) | Applies formats for a whole range. |
| [AutoFill](autofill)(Range) | Automaticall fill the target range. |
| [AutoFill](autofill)(Range, AutoFillType) | Automaticall fill the target range. |
| [Copy](copy)(Range) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [Copy](copy)(Range, PasteOptions) | Copying the range with paste special options. |
| [CopyData](copydata)(Range) | Copies cell data (including formulas) from a source range. |
| [CopyStyle](copystyle)(Range) | Copies style settings from a source range. |
| [CopyValue](copyvalue)(Range) | Copies cell value from a source range. |
| [ExportDataTable](exportdatatable)() | Exports data in this range to a DataTable object. |
| [ExportDataTable](exportdatatable)(ExportTableOptions) | Exports data in this range to a DataTable object. |
| [ExportDataTableAsString](exportdatatableasstring)() | Exports data in this range to a DataTable object. |
| [GetCellOrNull](getcellornull)(int, int) | Gets [`Cell`](../cell) object or null in this range. |
| [GetEnumerator](getenumerator)() | Gets the enumerator for cells in this Range. |
| [GetOffset](getoffset)(int, int) | Gets [`Range`](../range) range by offset. |
| [Intersect](intersect)(Range) | Returns a [`Range`](../range) object that represents the rectangular intersection of two ranges. |
| [IsIntersect](isintersect)(Range) | Indicates whether the range is intersect. |
| [Merge](merge)() | Combines a range of cells into a single cell. |
| [MoveTo](moveto)(int, int) | Move the current range to the dest range. |
| [PutValue](putvalue)(string, bool, bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [SetInsideBorders](setinsideborders)(BorderType, CellBorderType, CellsColor) | Set inside borders of the range. |
| [SetOutlineBorder](setoutlineborder)(BorderType, CellBorderType, Color) | Sets outline border around a range of cells. |
| [SetOutlineBorders](setoutlineborders)(CellBorderType, Color) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders](setoutlineborders)(CellBorderType[], Color[]) | Sets out line borders around a range of cells. |
| [SetStyle](setstyle)(Style) | Sets the style of the range. |
| override [ToString](tostring)() | Returns a string represents the current Range object. |
| [Union](union)(Range) | Returns the union of two ranges. |
| [UnMerge](unmerge)() | Unmerges merged cells of this range. |

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
