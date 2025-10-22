##Shape.HtmlText
Shape property. Gets and sets the html string which contains data and some formats in this textbox
## Shape.HtmlText property
Gets and sets the html string which contains data and some formats in this textbox.
```csharp
public string HtmlText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHtmlTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Check if HtmlText is empty and set it if needed
string html = shape.HtmlText;
if (string.IsNullOrEmpty(html))
{
shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
}
// Save the workbook
workbook.Save("ShapeHtmlTextDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
