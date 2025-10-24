##Cells.CopyRow
Cells method. Copies data and formats of a whole row
## Cells.CopyRow method
Copies data and formats of a whole row.
```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyRowWithCellsInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet1 = workbook.Worksheets[0];
Cells cells1 = worksheet1.Cells;
// Add some data to the first row
cells1["A1"].PutValue("Source Data");
cells1["B1"].PutValue(100);
cells1["C1"].PutValue(DateTime.Now);
// Create second worksheet
Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
Cells cells2 = worksheet2.Cells;
// Copy row from Sheet1 to Sheet2
cells2.CopyRow(cells1, 0, 0);
// Copy row within Sheet1 to new positions
cells1.CopyRow(cells1, 0, 1);
cells1.CopyRow(cells1, 0, 2);
// Save the workbook
workbook.Save("CopyRowExample.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
