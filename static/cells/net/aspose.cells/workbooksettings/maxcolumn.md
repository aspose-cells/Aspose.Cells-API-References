##WorkbookSettings.MaxColumn
WorkbookSettings property. Gets the max column index zerobased
## WorkbookSettings.MaxColumn property
Gets the max column index, zero-based.
```csharp
public int MaxColumn { get; }
```
### Remarks
Returns 255 if the file format is Excel97-2003;
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyMaxColumnDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Console.WriteLine("MaxColumn value: " + workbook.Settings.MaxColumn);
// Demonstrate MaxColumn usage by trying to access a column beyond the limit
try
{
Cells cells = workbook.Worksheets[0].Cells;
Cell cell = cells[0, workbook.Settings.MaxColumn + 1];
Console.WriteLine("This should not be reached");
}
catch (Exception ex)
{
Console.WriteLine("Expected error when accessing beyond MaxColumn: " + ex.Message);
}
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
