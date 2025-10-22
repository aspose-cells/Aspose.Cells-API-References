##Row.Index
Row property. Gets the index of this row
## Row.Index property
Gets the index of this row.
```csharp
public int Index { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Iterate through rows and demonstrate Index property
foreach (Row row in worksheet.Cells.Rows)
{
Console.WriteLine($"Processing row with index: {row.Index}");
if (row.Index > 0) // Skip header row
{
Console.WriteLine($"Data in row {row.Index}: " +
$"{worksheet.Cells[row.Index, 0].StringValue}, " +
$"{worksheet.Cells[row.Index, 1].IntValue}");
}
}
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
