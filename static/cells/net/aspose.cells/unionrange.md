##Class UnionRange
Aspose.Cells.UnionRange class. Represents union range
## UnionRange class
Represents union range.
```csharp
public class UnionRange : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Gets all cell count in the range. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Gets the count of rows in the range. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Gets the index of the first column of the range. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Gets the index of the first row of the range. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Indicates whether this has range. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Gets all hyperlink in the range. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Gets or sets the name of the range. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Gets the count of the ranges. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Gets all union ranges. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Gets the range's refers to. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Gets the count of rows in the range. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Gets and sets the values of the range. |
## Methods
| Name | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Applies formats for a whole range. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Copying the range with paste special options. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Gets the enumerator for cells in this Range. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Intersects another range. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Intersects another range. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Intersects another range. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Combines a range of cells into a single cell. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Sets out line borders around a range of cells. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Sets the style of the range. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Union the ranges. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Union another range. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Union another range. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Unmerges merged cells of this range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassUnionRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a union range using the correct API
UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
// Set value for the entire union range
unionRange.Value = "Test";
// Apply style to the union range
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.LightBlue;
unionRange.ApplyStyle(style, new StyleFlag { All = true });
// Save the workbook
workbook.Save("UnionRangeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
