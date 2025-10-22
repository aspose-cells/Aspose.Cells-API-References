##StyleFlag.ShrinkToFit
StyleFlag property. Shrink to fit setting will be applied
## StyleFlag.ShrinkToFit property
Shrink to fit setting will be applied.
```csharp
public bool ShrinkToFit { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyShrinkToFitDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set sample data in a cell
cells["A1"].PutValue("This is a long text that needs to fit in the cell");
// Create a style with ShrinkToFit enabled
Style style = workbook.CreateStyle();
style.ShrinkToFit = true;
// Create style flag and enable ShrinkToFit flag
StyleFlag flag = new StyleFlag();
flag.ShrinkToFit = true;
// Apply the style to the cell range (explicitly using Aspose.Cells.Range)
Aspose.Cells.Range range = cells.CreateRange("A1");
range.ApplyStyle(style, flag);
// Set column width to demonstrate shrinking
worksheet.Cells.SetColumnWidth(0, 10);
// Save the workbook
workbook.Save("ShrinkToFitDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
