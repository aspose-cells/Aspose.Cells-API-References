##Cells.TextToColumns
Cells method. Splits content in specified column into multiple columns
## Cells.TextToColumns method
Splits content in specified column into multiple columns..
```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| totalRows | Int32 | The number of rows. |
| options | TxtLoadOptions | The split options. |
### Return Value
Total column count of the split values.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set sample data with comma-separated values
sheet.Cells["A1"].PutValue("John,Doe,30");
sheet.Cells["A2"].PutValue("Jane,Smith,28");
// Create text load options with comma as separator
TxtLoadOptions options = new TxtLoadOptions();
options.Separator = ',';
// Split text to columns starting from cell A1, 3 columns wide
sheet.Cells.TextToColumns(0, 0, 3, options);
// Verify the results
Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
