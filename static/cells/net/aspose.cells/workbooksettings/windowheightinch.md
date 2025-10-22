##WorkbookSettings.WindowHeightInch
WorkbookSettings property. The height of the window in unit of inch
## WorkbookSettings.WindowHeightInch property
The height of the window, in unit of inch.
```csharp
public double WindowHeightInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowHeightInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set window height in inches
settings.WindowHeightInch = 5.5;
// Display the window height in inches
Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);
// Save the workbook
workbook.Save("WindowHeightInchDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
