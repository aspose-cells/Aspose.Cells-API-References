##Range.EntireColumn
Range property. Gets a Range object that represents the entire column or columns that contains the specified range
## Range.EntireColumn property
Gets a Range object that represents the entire column (or columns) that contains the specified range.
```csharp
public Range EntireColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyEntireColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a range starting at cell C1 (row 0, column 2)
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
// Get the entire column containing the range (column C)
Aspose.Cells.Range entireColumn = range.EntireColumn;
// Apply formatting to the entire column
Style style = entireColumn[0, 0].GetStyle();
style.Custom = "##0%";
StyleFlag styleFlag = new StyleFlag();
styleFlag.NumberFormat = true;
entireColumn.ApplyStyle(style, styleFlag);
// Save the workbook
workbook.Save("EntireColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
