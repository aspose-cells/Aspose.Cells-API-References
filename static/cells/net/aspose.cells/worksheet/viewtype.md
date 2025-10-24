##Worksheet.ViewType
Worksheet property. Gets and sets the view type
## Worksheet.ViewType property
Gets and sets the view type.
```csharp
public ViewType ViewType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyViewTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the view type to PageLayoutView and enable ruler
worksheet.ViewType = ViewType.PageLayoutView;
worksheet.IsRulerVisible = true;
// Add some sample content to demonstrate the view
worksheet.Cells["A1"].PutValue("Page Layout View Demo");
worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
// Save the workbook
workbook.Save("WorksheetViewTypeDemo.xlsx");
Console.WriteLine("Worksheet ViewType demo completed successfully.");
}
}
}
```
### See Also
* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
