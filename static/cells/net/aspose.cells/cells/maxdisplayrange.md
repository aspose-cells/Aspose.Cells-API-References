##Cells.MaxDisplayRange
Cells property. Gets the max range which includes data merged cells and shapes
## Cells.MaxDisplayRange property
Gets the max range which includes data, merged cells and shapes.
```csharp
public Range MaxDisplayRange { get; }
```
### Remarks
Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMaxDisplayRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells to create a display range
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["A3"].PutValue(300);
worksheet.Cells["B3"].PutValue(400);
// Get the max display range
Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;
// Output the range information
Console.WriteLine("Max Display Range:");
Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");
// Create a new range based on max display range dimensions
Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
maxDisplayRange.FirstRow,
maxDisplayRange.FirstColumn,
maxDisplayRange.RowCount,
maxDisplayRange.ColumnCount);
// Apply formatting to the range
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightGray;
style.Pattern = BackgroundType.Solid;
customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
// Save the workbook
workbook.Save("MaxDisplayRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
