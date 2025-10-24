##WorkbookSettings.IsHScrollBarVisible
WorkbookSettings property. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar
## WorkbookSettings.IsHScrollBarVisible property
Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.
```csharp
public bool IsHScrollBarVisible { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Hide the horizontal scroll bar
settings.IsHScrollBarVisible = false;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
