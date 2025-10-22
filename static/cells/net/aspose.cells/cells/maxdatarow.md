##Cells.MaxDataRow
Cells property. Maximum row index of cell which contains data
## Cells.MaxDataRow property
Maximum row index of cell which contains data.
```csharp
public int MaxDataRow { get; }
```
### Remarks
Return -1 if there is no cell which contains data. This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMaxDataRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("Item1");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue("Item2");
sheet.Cells["B3"].PutValue(20);
sheet.Cells["A4"].PutValue("Item3");
sheet.Cells["B4"].PutValue(30);
// Demonstrate MaxDataRow usage
int maxRow = sheet.Cells.MaxDataRow;
Console.WriteLine("Max data row: " + maxRow);
// Create a cell area using MaxDataRow
int startRow = 0;
int startColumn = 0;
int endRow = sheet.Cells.MaxDataRow;
int endColumn = sheet.Cells.MaxDataColumn;
// Apply formatting to the data range
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
// Apply style to the range
sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });
// Save the workbook
workbook.Save("MaxDataRowDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
