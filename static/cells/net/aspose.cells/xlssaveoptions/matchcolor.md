##XlsSaveOptions.MatchColor
XlsSaveOptions property. Indicates whether matching font color because there are 56 colors in the standard color palette
## XlsSaveOptions.MatchColor property
Indicates whether matching font color because there are 56 colors in the standard color palette.
```csharp
public bool MatchColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class XlsSaveOptionsPropertyMatchColorDemo
{
public static void Run()
{
// Create a workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B2 and set some text with specific font color
Cell cellB2 = worksheet.Cells["B2"];
cellB2.PutValue("Sample Text");
// Set font color to blue
Style style = cellB2.GetStyle();
style.Font.Color = Color.Blue;
cellB2.SetStyle(style);
// Create save options with MatchColor set to true
XlsSaveOptions saveOptions = new XlsSaveOptions();
saveOptions.MatchColor = true;
// Save the workbook with the options
workbook.Save("output.xls", saveOptions);
// Reload the saved file to verify the color was preserved
Workbook savedWorkbook = new Workbook("output.xls");
Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
// Verify the font color is still blue
Color savedColor = savedCellB2.GetStyle().Font.Color;
Console.WriteLine("Saved font color: " + savedColor.ToString());
}
}
}
```
### See Also
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
