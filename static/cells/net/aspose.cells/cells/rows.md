##Cells.Rows
Cells property. Gets the collection of Row objects that represents the individual rows in this worksheet
## Cells.Rows property
Gets the collection of [`Row`](../../row/) objects that represents the individual rows in this worksheet.
```csharp
public RowCollection Rows { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyRowsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set column width and row height
worksheet.Cells.SetColumnWidthPixel(0, 200);
worksheet.Cells.Rows[0].Height = 50;
// Access row properties through Rows collection
Row row = worksheet.Cells.Rows[0];
Console.WriteLine($"Row 0 height: {row.Height}");
Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
// Modify row properties
row.IsHeightMatched = true;
row.Height = 60;
// Verify changes
Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
// Save the workbook
workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
