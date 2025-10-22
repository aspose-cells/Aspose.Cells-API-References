##Class Outline
Aspose.Cells.Outline class. Represents an outline on a worksheet
## Outline class
Represents an outline on a worksheet.
```csharp
public class Outline
```
## Properties
| Name | Description |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Indicates if the summary column will be positioned to the right of the detail columns in the outline. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Indicates if the summary row will be positioned below the detail rows in the outline. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class OutlineDemo
{
public static void OutlineExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Access the outline of the worksheet
Outline outline = worksheet.Outline;
// Set the properties of the outline
outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
// Save the workbook
workbook.Save("OutlineExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
