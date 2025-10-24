##Cells.UngroupColumns
Cells method. Ungroups columns
## Cells.UngroupColumns method
Ungroups columns.
```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be ungrouped. |
| lastIndex | Int32 | The last column index to be ungrouped. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUngroupColumnsWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Group columns first to demonstrate ungrouping
worksheet.Cells.GroupColumns(0, 2);
// Ungroup columns (0 to 2)
worksheet.Cells.UngroupColumns(0, 2);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
