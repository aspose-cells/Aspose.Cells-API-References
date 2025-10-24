##Worksheet.Outline
Worksheet property. Gets the outline on this worksheet
## Worksheet.Outline property
Gets the outline on this worksheet.
```csharp
public Outline Outline { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyOutlineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and create outline groups
for (int i = 0; i < 10; i++)
{
worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
}
// Group rows (creates outline)
worksheet.Cells.GroupRows(0, 9, false);
// Access outline properties
Outline outline = worksheet.Outline;
Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");
// Change outline settings
outline.SummaryRowBelow = true;
outline.SummaryColumnRight = false;
// Ungroup rows to demonstrate outline functionality
worksheet.Cells.UngroupRows(0, 9);
// Save the workbook
workbook.Save("WorksheetOutlineDemo.xlsx");
}
}
}
```
### See Also
* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
