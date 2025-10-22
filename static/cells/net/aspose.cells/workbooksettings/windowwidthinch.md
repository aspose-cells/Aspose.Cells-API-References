##WorkbookSettings.WindowWidthInch
WorkbookSettings property. The width of the window in unit of inch
## WorkbookSettings.WindowWidthInch property
The width of the window, in unit of inch.
```csharp
public double WindowWidthInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowWidthInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set window width in inches
settings.WindowWidthInch = 10.5;
// Display the window width in inches
Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);
// Save the workbook
workbook.Save("WindowWidthInchDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
