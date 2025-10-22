##WorkbookSettings.SheetTabBarWidth
WorkbookSettings property. Width of worksheet tab bar in 1/1000 of window width
## WorkbookSettings.SheetTabBarWidth property
Width of worksheet tab bar (in 1/1000 of window width).
```csharp
public int SheetTabBarWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertySheetTabBarWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the SheetTabBarWidth property
workbook.Settings.SheetTabBarWidth = 1000;
// Get and display the SheetTabBarWidth value
Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
