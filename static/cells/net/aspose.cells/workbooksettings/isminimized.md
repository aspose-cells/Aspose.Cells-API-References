##WorkbookSettings.IsMinimized
WorkbookSettings property. Represents whether the generated spreadsheet will be opened Minimized
## WorkbookSettings.IsMinimized property
Represents whether the generated spreadsheet will be opened Minimized.
```csharp
public bool IsMinimized { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsMinimizedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set IsMinimized property to true
workbook.Settings.IsMinimized = true;
// Save the workbook
workbook.Save("IsMinimizedDemo.xlsx");
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");
// Output the IsMinimized property value
Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
