##Worksheet.IsGridlinesVisible
Worksheet property. Gets or sets a value indicating whether the gridlines are visible.Default is true
## Worksheet.IsGridlinesVisible property
Gets or sets a value indicating whether the gridlines are visible.Default is true.
```csharp
public bool IsGridlinesVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsGridlinesVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set gridlines visibility to true
worksheet.IsGridlinesVisible = true;
// Add some sample data to see gridlines
worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
// Auto-fit columns for better visibility
worksheet.AutoFitColumns();
// Save the workbook
workbook.Save("GridlinesVisibleDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
