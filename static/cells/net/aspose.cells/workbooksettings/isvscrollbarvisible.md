##WorkbookSettings.IsVScrollBarVisible
WorkbookSettings property. Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar
## WorkbookSettings.IsVScrollBarVisible property
Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.
```csharp
public bool IsVScrollBarVisible { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Hide the vertical scroll bar
settings.IsVScrollBarVisible = false;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
