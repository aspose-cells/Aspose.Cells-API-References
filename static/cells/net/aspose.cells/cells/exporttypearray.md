##Cells.ExportTypeArray
Cells method. Exports cell value type in the Cells collection to a twodimension array object
## Cells.ExportTypeArray method
Exports cell value type in the [`Cells`](../) collection to a two-dimension array object.
```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows,
int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be exported. |
| totalColumns | Int32 | Number of columns to be exported. |
### Return Value
Exported array object representing cell value types.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values in cells
cells["A1"].PutValue(10);
cells["B1"].PutValue("Hello");
cells["A2"].PutValue(true);
cells["B2"].PutValue(DateTime.Now);
// Export cell types to a 2D array
CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);
// Display the results
for (int i = 0; i < 2; i++)
{
for (int j = 0; j < 2; j++)
{
Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
}
}
// Demonstrate exception case
try
{
CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
}
catch (CellsException ex)
{
Console.WriteLine("Exception caught as expected: " + ex.Message);
}
}
}
}
```
### See Also
* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
