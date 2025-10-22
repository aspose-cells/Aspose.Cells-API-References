##WorkbookSettings.UpdateLinksType
WorkbookSettings property. Gets and sets how updates external links when the workbook is opened
## WorkbookSettings.UpdateLinksType property
Gets and sets how updates external links when the workbook is opened.
```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyUpdateLinksTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the UpdateLinksType to Never
workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the setting
Workbook loadedWorkbook = new Workbook("output.xlsx");
// Output the UpdateLinksType value
Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
}
}
}
```
### See Also
* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
