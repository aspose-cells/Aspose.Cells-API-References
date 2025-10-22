##Cells.UnMerge
Cells method. Unmerges a specified range of merged cells
## Cells.UnMerge method
Unmerges a specified range of merged cells.
```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Merge cells first
cells.Merge(0, 0, 2, 2);
// Unmerge the previously merged cells
cells.UnMerge(0, 0, 2, 2);
// Save the workbook
workbook.Save("UnMergeDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
