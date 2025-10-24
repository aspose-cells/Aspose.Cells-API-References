##Cells.MaxDataColumn
Cells property. Maximum column index of cell which contains data
## Cells.MaxDataColumn property
Maximum column index of cell which contains data.
```csharp
public int MaxDataColumn { get; }
```
### Remarks
-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Data;
namespace AsposeCellsExamples
{
public class CellsPropertyMaxDataColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["A3"].PutValue(300);
worksheet.Cells["B3"].PutValue(400);
// Get the maximum data column index (0-based)
int maxColumn = worksheet.Cells.MaxDataColumn;
Console.WriteLine("Max Data Column: " + maxColumn);
// Export data using MaxDataColumn
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0,
worksheet.Cells.MaxDataRow + 1,
worksheet.Cells.MaxDataColumn + 1);
// Display exported data
Console.WriteLine("Exported Data:");
foreach (DataRow row in dataTable.Rows)
{
for (int i = 0; i <= maxColumn; i++)
{
Console.Write(row[i] + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
