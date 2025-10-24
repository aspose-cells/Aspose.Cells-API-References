##Cells.ExportArray
Cells method. Exports data in the Cells collection to a twodimension array object
## Cells.ExportArray method
Exports data in the [`Cells`](../) collection to a two-dimension array object.
```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be exported |
| totalColumns | Int32 | Number of columns to be exported |
### Return Value
Exported cell value array object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some sample data
cells[0, 0].PutValue("A");
cells[0, 1].PutValue("B");
cells[1, 0].PutValue(10);
cells[1, 1].PutValue(20);
try
{
// Export data to array
object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
// Display the exported array
for (int i = 0; i < 2; i++)
{
for (int j = 0; j < 2; j++)
{
Console.Write(dataArray[i, j] + "\t");
}
Console.WriteLine();
}
}
catch (CellsException ex)
{
Console.WriteLine("Error exporting array: " + ex.Message);
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
