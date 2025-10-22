##Cells.UngroupRows
Cells method. Ungroups rows
## UngroupRows(int, int, bool) {#ungrouprows_1}
Ungroups rows.
```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be ungrouped. |
| lastIndex | Int32 | The last row index to be ungrouped. |
| isAll | Boolean | True, removes all grouped info.Otherwise, remove the outer group info. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create nested row groupings for demonstration
worksheet.Cells.GroupRows(5, 7);  // First level grouping
worksheet.Cells.GroupRows(5, 7);  // Second level grouping
try
{
// Ungroup all levels of rows 5-7
worksheet.Cells.UngroupRows(5, 7, true);
Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
}
// Save the modified workbook
workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## UngroupRows(int, int) {#ungrouprows}
Ungroups rows.
```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be ungrouped. |
| lastIndex | Int32 | The last row index to be ungrouped. |
### Remarks
Only removes outer group info.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUngroupRowsWithInt32Int32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some data
for (int i = 0; i < 6; i++)
{
cells[i, 0].PutValue($"Row {i}");
}
// Group rows 1 through 3 (0-based index)
cells.GroupRows(1, 3, true);
Console.WriteLine("Rows grouped from index 1 to 3");
// Ungroup the same rows
cells.UngroupRows(1, 3);
Console.WriteLine("Rows ungrouped from index 1 to 3");
// Save the workbook
workbook.Save("UngroupRowsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
