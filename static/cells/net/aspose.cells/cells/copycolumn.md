##Cells.CopyColumn
Cells method. Copies data and formats of a whole column
## Cells.CopyColumn method
Copies data and formats of a whole column.
```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyColumnWithCellsInt32Int32Demo
{
public static void Run()
{
// Create source workbook and populate data
Workbook wbSrc = new Workbook();
Cells cellsSrc = wbSrc.Worksheets[0].Cells;
cellsSrc[0, 255].PutValue(1);
cellsSrc[1, 255].PutValue(true);
cellsSrc[2, 255].PutValue("abc");
cellsSrc[3, 255].PutValue(false);
cellsSrc[65535, 255].PutValue(2.56);
// Create destination workbook
Workbook wbDest = new Workbook();
Cells cellsDest = wbDest.Worksheets[0].Cells;
// Copy column from source to destination
cellsDest.CopyColumn(cellsSrc, 255, 0);
// Save the result
wbDest.Save("outputCopyColumn.xlsx");
Console.WriteLine("Column copied successfully.");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
