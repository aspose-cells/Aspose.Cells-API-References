##Worksheet.UnFreezePanes
Worksheet method. Unfreezes panes in the worksheet
## Worksheet.UnFreezePanes method
Unfreezes panes in the worksheet.
```csharp
public void UnFreezePanes()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodUnFreezePanesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Freeze panes at cell C3 (rows 2, columns 2 frozen)
worksheet.FreezePanes("C3", 2, 2);
// Verify panes are frozen
int frozenRow, frozenColumn, frozenRows, frozenColumns;
worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");
// Unfreeze the panes
worksheet.UnFreezePanes();
// Verify panes are unfrozen
worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");
// Save the workbook
workbook.Save("UnFreezePanesDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
