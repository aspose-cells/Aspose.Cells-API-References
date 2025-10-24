##DefaultStyleSettings.VerticalAlignment
DefaultStyleSettings property. Gets/Sets the default value for vertical alignment
## DefaultStyleSettings.VerticalAlignment property
Gets/Sets the default value for vertical alignment
```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set default vertical alignment to Bottom
LoadOptions options = new LoadOptions();
options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
worksheet.Cells["A1"].PutValue("Sample Text 1");
worksheet.Cells["B1"].PutValue("Sample Text 2");
worksheet.Cells["C1"].PutValue("Sample Text 3");
// Verify the vertical alignment is applied to all cells
foreach (Cell cell in worksheet.Cells)
{
Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
}
// Save the workbook
workbook.Save("VerticalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
