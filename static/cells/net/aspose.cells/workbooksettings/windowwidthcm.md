##WorkbookSettings.WindowWidthCM
WorkbookSettings property. The width of the window in unit of centimeter
## WorkbookSettings.WindowWidthCM property
The width of the window, in unit of centimeter.
```csharp
public double WindowWidthCM { get; set; }
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowWidthCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowWidthCM property (20.32 cm = ~8 inches)
settings.WindowWidthCM = 20.32;
// Verify the setting by printing it
Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
// Save the workbook
workbook.Save("WindowWidthCMDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
