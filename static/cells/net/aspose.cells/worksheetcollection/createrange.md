##WorksheetCollection.CreateRange
WorksheetCollection method. Creates a Range object from an address of the range
## WorksheetCollection.CreateRange method
Creates a [`Range`](../../range/) object from an address of the range.
```csharp
public Range CreateRange(string address, int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Int32 | The sheet index. |
### Return Value
A [`Range`](../../range/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 6; j++)
{
worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
}
}
// Create range using string address and sheet index
Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);
// Demonstrate range usage
Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
