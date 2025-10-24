##WorkbookSettings.WindowLeftInch
WorkbookSettings property. The distance from the left edge of the client area to the left edge of the window. In unit of inch
## WorkbookSettings.WindowLeftInch property
The distance from the left edge of the client area to the left edge of the window. In unit of inch.
```csharp
public double WindowLeftInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowLeftInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowLeftInch property
settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen
// Add some sample data to demonstrate workbook is functional
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Window Position Demo");
sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");
// Save the workbook
workbook.Save("WindowLeftInchDemo.xlsx");
Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
