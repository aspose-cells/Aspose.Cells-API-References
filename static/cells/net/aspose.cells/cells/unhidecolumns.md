##Cells.UnhideColumns
Cells method. Unhide multiple columns
## Cells.UnhideColumns method
Unhide multiple columns.
```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| totalColumns | Int32 | Column number |
| width | Double | Column width. |
### Remarks
Only applies the column width to the hidden columns.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Hide columns 1-3 (zero-based) initially
worksheet.Cells.HideColumns(1, 3);
try
{
// Unhide columns starting at index 1 (second column), 3 columns wide, set width to 15.5
worksheet.Cells.UnhideColumns(1, 3, 15.5);
// Verify unhidden columns by checking their width
Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
}
// Save the modified workbook
workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
