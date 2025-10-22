##WorkbookSettings.WindowHeight
WorkbookSettings property. The height of the window in unit of point
## WorkbookSettings.WindowHeight property
The height of the window, in unit of point.
```csharp
public double WindowHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowHeight property
settings.WindowHeight = 600;
// Verify the WindowHeight value
Console.WriteLine("Window Height set to: " + settings.WindowHeight);
// Save the workbook
workbook.Save("WindowHeightDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
