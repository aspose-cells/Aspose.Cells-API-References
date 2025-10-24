##WorkbookSettings.CrashSave
WorkbookSettings property. indicates whether the application last saved the workbook file after a crash
## WorkbookSettings.CrashSave property
indicates whether the application last saved the workbook file after a crash.
```csharp
public bool CrashSave { get; set; }
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyCrashSaveDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("CrashSave Demo");
sheet.Cells["A2"].PutValue(DateTime.Now);
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Demonstrate CrashSave property
settings.CrashSave = true;
Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");
// Save with crash save enabled
workbook.Save("CrashSaveEnabled.xlsx");
// Disable crash save
settings.CrashSave = false;
Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");
// Save with crash save disabled
workbook.Save("CrashSaveDisabled.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
