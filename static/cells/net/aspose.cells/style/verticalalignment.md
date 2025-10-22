##Style.VerticalAlignment
Style property. Gets or sets the vertical alignment type of the text in a cell
## Style.VerticalAlignment property
Gets or sets the vertical alignment type of the text in a cell.
```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyVerticalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1
Cell cell = worksheet.Cells["A1"];
// Set the cell value
cell.PutValue("Vertical Alignment Demo");
// Access the cell's style
Style style = cell.GetStyle();
// Set vertical alignment to Top
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);
// Save the workbook
workbook.Save("VerticalAlignmentDemo.xlsx");
Console.WriteLine("Vertical alignment set to Top for cell A1.");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
