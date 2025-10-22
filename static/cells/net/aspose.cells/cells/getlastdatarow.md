##Cells.GetLastDataRow
Cells method. Gets the last row index of cell which contains data in the specified column
## Cells.GetLastDataRow method
Gets the last row index of cell which contains data in the specified column.
```csharp
public int GetLastDataRow(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
### Return Value
last row index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetLastDataRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
worksheet.Cells["A4"].PutValue("Data3");
// Get the last data row in column A (index 0)
int lastRow = worksheet.Cells.GetLastDataRow(0);
// Output the result
Console.WriteLine("Last data row in column A: " + lastRow);
// Insert a new row after the last data row
CellArea area = new CellArea();
area.StartRow = lastRow + 1;
area.EndRow = lastRow + 1;
area.StartColumn = 0;
area.EndColumn = 0;
worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
// Add data to the new row
worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
