##Range.FirstColumn
Range property. Gets the index of the first column of the range
## Range.FirstColumn property
Gets the index of the first column of the range.
```csharp
public int FirstColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyFirstColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
// Create a range
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
// Demonstrate FirstColumn property
Console.WriteLine("First column index of range: " + range.FirstColumn);
// Use FirstColumn to access cells in the first column of the range
for (int i = 0; i < range.RowCount; i++)
{
Cell cell = range[i, 0]; // Access first column (index 0) of the range
Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
}
// Save the workbook
workbook.Save("RangeFirstColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
