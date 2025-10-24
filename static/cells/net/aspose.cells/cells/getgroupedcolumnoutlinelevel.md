##Cells.GetGroupedColumnOutlineLevel
Cells method. Gets the outline level zerobased of the column
## Cells.GetGroupedColumnOutlineLevel method
Gets the outline level (zero-based) of the column.
```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | The column index |
### Return Value
The outline level of the column
### Remarks
If the column is not grouped, returns zero.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Group columns (first 3 columns) without hiding them
worksheet.Cells.GroupColumns(0, 2, false);
// Get outline level of first column
int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
Console.WriteLine("Outline level of column 0: " + outlineLevel);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
