##Cells.ShowGroupDetail
Cells method. Expands the grouped rows/columns
## Cells.ShowGroupDetail method
Expands the grouped rows/columns.
```csharp
public void ShowGroupDetail(bool isVertical, int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isVertical | Boolean | True, expands the grouped rows. |
| index | Int32 | The row/column index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodShowGroupDetailWithBooleanInt32Demo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data in rows 5-7 (zero-based index 4-6)
for (int row = 4; row <= 6; row++)
{
worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
}
// Group rows 4-6 (Excel rows 5-7) and collapse them initially
worksheet.Cells.GroupRows(4, 6, true);
try
{
// Expand the grouped rows using ShowGroupDetail (isVertical: false for rows, index: 4)
worksheet.Cells.ShowGroupDetail(false, 4);
Console.WriteLine("ShowGroupDetail method executed successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
}
// Save the workbook to demonstrate the effect
workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
