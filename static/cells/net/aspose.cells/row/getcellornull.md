##Row.GetCellOrNull
Row method. Gets the cell or null in the specific index
## Row.GetCellOrNull method
Gets the cell or null in the specific index.
```csharp
public Cell GetCellOrNull(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index |
### Return Value
Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowMethodGetCellOrNullWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add sample data
ws.Cells["A1"].PutValue("Header1");
ws.Cells["B1"].PutValue("Header2");
ws.Cells["A2"].PutValue(100);
ws.Cells["B2"].PutValue(200);
// Get the first row
Row row = ws.Cells.Rows[0];
// Demonstrate GetCellOrNull with Int32 parameter
for (int colIndex = 0; colIndex < 2; colIndex++)
{
Cell cell = row.GetCellOrNull(colIndex);
if (cell != null)
{
Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
}
else
{
Console.WriteLine($"Cell at column {colIndex} is null");
}
}
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
