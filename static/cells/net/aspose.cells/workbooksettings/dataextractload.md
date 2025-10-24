##WorkbookSettings.DataExtractLoad
WorkbookSettings property. indicates whether the application last opened the workbook for data recovery
## WorkbookSettings.DataExtractLoad property
indicates whether the application last opened the workbook for data recovery.
```csharp
public bool DataExtractLoad { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyDataExtractLoadDemo
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
string destPath = "output.xlsx";
workbook.Save(destPath);
// Reload the workbook to verify settings
Workbook loadedWorkbook = new Workbook(destPath);
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
