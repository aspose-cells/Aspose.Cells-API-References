##Worksheet.IsRowColumnHeadersVisible
Worksheet property. Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true
## Worksheet.IsRowColumnHeadersVisible property
Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.
```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set row and column headers visibility to false
worksheet.IsRowColumnHeadersVisible = false;
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Output the property value
Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
