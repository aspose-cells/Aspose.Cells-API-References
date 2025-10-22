##WorkbookSettings.SetPageOrientationType
WorkbookSettings method. Set the type of print orientation for the whole workbook
## WorkbookSettings.SetPageOrientationType method
Set the type of print orientation for the whole workbook.
```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | The page orientation type |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
workbook.Worksheets.Add();
// Set page orientation to Portrait for all worksheets
workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
// Verify the orientation is set correctly
foreach (Worksheet sheet in workbook.Worksheets)
{
Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
}
}
}
}
```
### See Also
* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
