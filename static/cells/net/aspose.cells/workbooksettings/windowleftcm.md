##WorkbookSettings.WindowLeftCM
WorkbookSettings property. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter
## WorkbookSettings.WindowLeftCM property
The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.
```csharp
public double WindowLeftCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWindowLeftCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set WindowLeftCM property (distance from left edge of screen in centimeters)
settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm
// Verify the setting by printing it
Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);
// Save the workbook
workbook.Save("WindowLeftCMDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
