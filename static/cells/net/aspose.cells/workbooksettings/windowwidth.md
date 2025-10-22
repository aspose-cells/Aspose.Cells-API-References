##WorkbookSettings.WindowWidth
WorkbookSettings property. The width of the window in unit of point
## WorkbookSettings.WindowWidth property
The width of the window, in unit of point.
```csharp
public double WindowWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set the WindowWidth property
settings.WindowWidth = 800;
// Verify the WindowWidth value
Console.WriteLine("Window Width set to: " + settings.WindowWidth);
// Save the workbook
workbook.Save("WindowWidthDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
