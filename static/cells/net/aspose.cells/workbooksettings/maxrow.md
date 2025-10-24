##WorkbookSettings.MaxRow
WorkbookSettings property. Gets the max row index zerobased
## WorkbookSettings.MaxRow property
Gets the max row index, zero-based.
```csharp
public int MaxRow { get; }
```
### Remarks
Returns 65535 if the file format is Excel97-2003;
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyMaxRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate MaxRow property
Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
// Try to access a cell beyond MaxRow (should throw exception)
try
{
Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
Console.WriteLine("This line shouldn't execute");
}
catch (Exception ex)
{
Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
}
// Create a cell area using MaxRow
CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
