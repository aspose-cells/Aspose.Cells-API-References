##Style.Pattern
Style property. Gets or sets the cell background pattern type
## Style.Pattern property
Gets or sets the cell background pattern type.
```csharp
public BackgroundType Pattern { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyPatternDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access cell and get its style
Cell cell = cells[0, 0];
Style style = cell.GetStyle();
// Set pattern and foreground color
style.Pattern = BackgroundType.Gray50;
style.ForegroundColor = System.Drawing.Color.LightGray;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("PatternPropertyDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
