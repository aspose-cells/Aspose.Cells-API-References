##WorkbookSettings.WindowTopInch
WorkbookSettings property. The distance from the top edge of the client area to the top edge of the window in unit of inch
## WorkbookSettings.WindowTopInch property
The distance from the top edge of the client area to the top edge of the window, in unit of inch.
```csharp
public double WindowTopInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowTopInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowTopInch property to position the window 2 inches from top
settings.WindowTopInch = 2.0;
// Verify the setting by printing it
Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);
// Save the workbook
workbook.Save("WindowTopInchDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
