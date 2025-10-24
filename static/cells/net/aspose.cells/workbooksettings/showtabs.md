##WorkbookSettings.ShowTabs
WorkbookSettings property. Get or sets a value whether the Workbook tabs are displayed
## WorkbookSettings.ShowTabs property
Get or sets a value whether the Workbook tabs are displayed.
```csharp
public bool ShowTabs { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyShowTabsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Hide the spreadsheet tabs
workbook.Settings.ShowTabs = false;
// Save the workbook
workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
// Create another workbook to show tabs
Workbook workbook2 = new Workbook();
// Ensure tabs are visible (default is true)
workbook2.Settings.ShowTabs = true;
// Save the workbook
workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
