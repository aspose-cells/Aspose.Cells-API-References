##WorkbookSettings.CheckCustomNumberFormat
WorkbookSettings property. Indicates whether checking custom number format when setting Style.Custom
## WorkbookSettings.CheckCustomNumberFormat property
Indicates whether checking custom number format when setting Style.Custom.
```csharp
public bool CheckCustomNumberFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style style = workbook.CreateStyle();
// First set a valid custom number format
style.Custom = "#,##0.00";
// Enable strict checking
workbook.Settings.CheckCustomNumberFormat = true;
try
{
// Attempt to set an invalid custom number format
style.Custom = "fff @ ggg";
}
catch (CellsException ex)
{
Console.WriteLine("Error setting custom format: " + ex.Message);
}
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
