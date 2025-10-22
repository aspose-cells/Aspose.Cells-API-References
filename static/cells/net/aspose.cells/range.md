##Class Range
Aspose.Cells.Range class. Encapsulates the object that represents a range of cells within a spreadsheet
## Range class
Encapsulates the object that represents a range of cells within a spreadsheet.
```csharp
public class Range : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Gets address of the range. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Gets the count of columns in the range. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Sets or gets the column width of this range |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Gets the index of the first column of the range. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Gets the index of the first row of the range. |
| [Height](../../aspose.cells/range/height/) { get; } | Gets the width of a range in points. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Gets all hyperlink in the range. |
| [Item](../../aspose.cells/range/item/) { get; } | Gets [`Cell`](../cell/) object in this range. |
| [Left](../../aspose.cells/range/left/) { get; } | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Gets or sets the name of the range. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Gets the range's refers to. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Gets the count of rows in the range. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Sets or gets the height of rows in this range |
| [Top](../../aspose.cells/range/top/) { get; } | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Gets and sets the value of the range. |
| [Width](../../aspose.cells/range/width/) { get; } | Gets the width of a range in points. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Gets the [`Worksheet`](./worksheet/)object which contains this range. |
## Methods
| Name | Description |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Adds a hyperlink to a specified cell or a range of cells. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Applies formats for a whole range. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Automaticall fill the target range. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Automaticall fill the target range. |
| [Clear](../../aspose.cells/range/clear/)() | Clears this range. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Clears the comments of this range. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Clears the contents of this range. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Clears the formats of this range. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Only removes hyperlinks. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Copying the range with paste special options. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Copies cell data (including formulas) from a source range. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Copies style settings from a source range. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Copies cell value from a source range. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Exports data in this range to a DataTable object. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Exports data in this range to a DataTable object. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Exports data in this range to a DataTable object. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Gets [`Cell`](../cell/) object or null in this range. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Gets the enumerator for cells in this Range. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Gets `Range` range by offset. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Returns a `Range` object that represents the rectangular intersection of two ranges. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Indicates whether the range contains values. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Indicates whether the range is intersect. |
| [Merge](../../aspose.cells/range/merge/)() | Combines a range of cells into a single cell. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Move the current range to the dest range. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Set inside borders of the range. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Sets outline border around a range of cells. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Sets outline border around a range of cells. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Sets out line borders around a range of cells. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Sets the style of the range. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Apply the cell style. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Convert the range to html . |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Converts the range to image. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Convert the range to JSON value. |
| override [ToString](../../aspose.cells/range/tostring/)() | Returns a string represents the current Range object. |
| [Transpose](../../aspose.cells/range/transpose/)() | Transpose (rotate) data from rows to columns or vice versa. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) Returns the union of two ranges. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) Returns the union result of two ranges. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Returns the union result of two ranges. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Unmerges merged cells of this range. |
### Remarks
The Range class denotes a region of Excel spreadsheet. With this, you can format and set value of the range. And you can simply copy range of Excel too.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
range.Value = "Hello";
workbook.Save("book1.xlsm");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
