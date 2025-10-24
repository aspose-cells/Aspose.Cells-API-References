##WorkbookSettings.WindowHeightCM
WorkbookSettings property. The height of the window in unit of centimeter
## WorkbookSettings.WindowHeightCM property
The height of the window, in unit of centimeter.
```csharp
public double WindowHeightCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowHeightCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set WindowHeightCM property
settings.WindowHeightCM = 15.5;
// Display the set value
Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);
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
