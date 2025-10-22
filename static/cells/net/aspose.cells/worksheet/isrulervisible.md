##Worksheet.IsRulerVisible
Worksheet property. Indicates whether the ruler is visible. This property is only applied for page break preview
## Worksheet.IsRulerVisible property
Indicates whether the ruler is visible. This property is only applied for page break preview.
```csharp
public bool IsRulerVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsRulerVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the worksheet to PageLayoutView where ruler is visible
worksheet.ViewType = ViewType.PageLayoutView;
// Toggle ruler visibility
worksheet.IsRulerVisible = true;
// Output the current ruler visibility state
Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);
// Save the workbook
workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
