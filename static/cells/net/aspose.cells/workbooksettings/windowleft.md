##WorkbookSettings.WindowLeft
WorkbookSettings property. The distance from the left edge of the client area to the left edge of the window in unit of point
## WorkbookSettings.WindowLeft property
The distance from the left edge of the client area to the left edge of the window, in unit of point.
```csharp
public double WindowLeft { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowLeftDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowLeft property to position the window 100 pixels from left
settings.WindowLeft = 100;
// Set other window properties for demonstration
settings.WindowTop = 50;
settings.WindowWidth = 800;
settings.WindowHeight = 600;
// Add sample data to worksheet
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Window Position Demo");
sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");
// Save the workbook
workbook.Save("WindowPositionDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
