##WorkbookSettings.IsHidden
WorkbookSettings property. Indicates whether this workbook is hidden
## WorkbookSettings.IsHidden property
Indicates whether this workbook is hidden.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set IsHidden property to true
settings.IsHidden = true;
Console.WriteLine("Workbook is hidden: " + settings.IsHidden);
// Save the workbook
workbook.Save("WorkbookSettings_IsHidden_True.xlsx");
// Create another workbook
Workbook workbook2 = new Workbook();
// Access workbook settings
WorkbookSettings settings2 = workbook2.Settings;
// Set IsHidden property to false (default)
settings2.IsHidden = false;
Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);
// Save the workbook
workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");
// Load and check the saved workbooks
Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);
Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
