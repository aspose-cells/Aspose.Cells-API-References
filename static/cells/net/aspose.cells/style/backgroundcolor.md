##Style.BackgroundColor
Style property. Gets or sets a styles background color
## Style.BackgroundColor property
Gets or sets a style's background color.
```csharp
public Color BackgroundColor { get; set; }
```
### Remarks
If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyBackgroundColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a style object
Style style = workbook.CreateStyle();
// Set background color to yellow
style.BackgroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
// Apply the style to cell A1
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Cell with yellow background");
cell.SetStyle(style);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
