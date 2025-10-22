##Cells.LastCell
Cells property. Gets the last cell in this worksheet
## Cells.LastCell property
Gets the last cell in this worksheet.
```csharp
public Cell LastCell { get; }
```
### Remarks
Returns null if there is no data in the worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyLastCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].Value = "Header1";
worksheet.Cells["B1"].Value = "Header2";
worksheet.Cells["A2"].Value = "Data1";
worksheet.Cells["B2"].Value = "Data2";
// Get the last cell address
Cell lastCell = worksheet.Cells.LastCell;
Console.WriteLine("Last cell address: " + lastCell.Name);
// Create a range from first to last cell
Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
worksheet.Cells.FirstCell.Name,
lastCell.Name);
// Apply formatting to the range
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });
// Save the workbook
workbook.Save("LastCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
