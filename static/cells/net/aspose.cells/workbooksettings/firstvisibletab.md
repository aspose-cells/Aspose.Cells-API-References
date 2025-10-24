##WorkbookSettings.FirstVisibleTab
WorkbookSettings property. Gets or sets the first visible worksheet tab
## WorkbookSettings.FirstVisibleTab property
Gets or sets the first visible worksheet tab.
```csharp
public int FirstVisibleTab { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyFirstVisibleTabDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Set the first visible tab index (0-based)
workbook.Settings.FirstVisibleTab = 1;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
// Verify the setting
Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
