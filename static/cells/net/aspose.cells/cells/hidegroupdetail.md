##Cells.HideGroupDetail
Cells method. Collapses the grouped rows/columns
## Cells.HideGroupDetail method
Collapses the grouped rows/columns.
```csharp
public void HideGroupDetail(bool isVertical, int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | Boolean | True, collapse the grouped rows. |
| index | Int32 | The row/column index |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodHideGroupDetailWithBooleanInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Group rows and hide details
worksheet.Cells.GroupRows(0, 9, false);
worksheet.Cells.HideGroupDetail(true, 4);
worksheet.Cells.HideGroupDetail(true, 7);
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
