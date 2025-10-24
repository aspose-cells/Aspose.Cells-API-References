##WorkbookSettings.RepairLoad
WorkbookSettings property. Indicates whether the application last opened the workbook in safe or repair mode
## WorkbookSettings.RepairLoad property
Indicates whether the application last opened the workbook in safe or repair mode.
```csharp
public bool RepairLoad { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyRepairLoadDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Configure workbook settings
workbook.Settings.AutoRecover = false;
workbook.Settings.DataExtractLoad = true;
workbook.Settings.CrashSave = true;
workbook.Settings.RepairLoad = true;
// Save the workbook
string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
workbook.Save(outputPath);
// Load the saved workbook to verify settings
Workbook loadedWorkbook = new Workbook(outputPath);
// Output the settings to console
Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
