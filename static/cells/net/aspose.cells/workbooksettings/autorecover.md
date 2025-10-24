##WorkbookSettings.AutoRecover
WorkbookSettings property. Indicates whether the file is marked for autorecovery
## WorkbookSettings.AutoRecover property
Indicates whether the file is marked for auto-recovery.
```csharp
public bool AutoRecover { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyAutoRecoverDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set AutoRecover and other settings
workbook.Settings.AutoRecover = false;
workbook.Settings.DataExtractLoad = true;
workbook.Settings.CrashSave = true;
workbook.Settings.RepairLoad = true;
// Save the workbook
string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
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
