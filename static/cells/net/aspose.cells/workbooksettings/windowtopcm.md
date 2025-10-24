##WorkbookSettings.WindowTopCM
WorkbookSettings property. The distance from the top edge of the client area to the top edge of the window in unit of centimeter
## WorkbookSettings.WindowTopCM property
The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.
```csharp
public double WindowTopCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowTopCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set WindowTopCM property (position from top in centimeters)
settings.WindowTopCM = 2.5;
// Display the current WindowTopCM value
Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);
// Save the workbook
workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
