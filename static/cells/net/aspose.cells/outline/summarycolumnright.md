##Outline.SummaryColumnRight
Outline property. Indicates if the summary column will be positioned to the right of the detail columns in the outline
## Outline.SummaryColumnRight property
Indicates if the summary column will be positioned to the right of the detail columns in the outline.
```csharp
public bool SummaryColumnRight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OutlinePropertySummaryColumnRightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and group rows
for (int i = 0; i < 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
}
// Group rows (creates an outline)
worksheet.Cells.GroupRows(0, 9, false);
// Get the outline settings
Outline outline = worksheet.Outline;
// Set SummaryColumnRight to true (summary columns will appear to the right of detail columns)
outline.SummaryColumnRight = true;
Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);
// Save the workbook
workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
}
}
}
```
### See Also
* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
