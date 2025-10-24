##Worksheet.GetFreezedPanes
Worksheet method. Gets the freeze panes
## Worksheet.GetFreezedPanes method
Gets the freeze panes.
```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows,
out int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32& | Row index. |
| column | Int32& | Column index. |
| freezedRows | Int32& | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32& | Number of visible columns in left pane, no more than column index. |
### Return Value
Return whether the worksheet is frozen
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Freeze panes at cell C5 (row 4, column 2) with 2 frozen rows and 1 frozen column
worksheet.FreezePanes(4, 2, 2, 1);
// Declare variables to store the freeze pane information
int row = 0;
int column = 0;
int freezedRows = 0;
int freezedColumns = 0;
try
{
// Call the GetFreezedPanes method with out parameters
bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);
// Display the results
Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
if (hasFreeze)
{
Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
}
// Save the workbook
workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
