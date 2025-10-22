##Worksheet.IsVisible
Worksheet property. Represents if the worksheet is visible
## Worksheet.IsVisible property
Represents if the worksheet is visible.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add 3 worksheets
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Set the second worksheet to be hidden
workbook.Worksheets[1].IsVisible = false;
// Save the workbook
workbook.Save("WorksheetVisibilityDemo.xlsx");
// Display visibility status
Console.WriteLine("Worksheet Visibility Status:");
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
}
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
