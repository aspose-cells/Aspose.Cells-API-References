##TextOptions.FarEastName
TextOptions property. Gets and sets the FarEast name
## TextOptions.FarEastName property
Gets and sets the FarEast name.
```csharp
public string FarEastName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextOptionsPropertyFarEastNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set FarEastName font
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
shape.Text = "Sample Text";
shape.TextOptions.FarEastName = "宋体";
// Save and reload to verify
string outputPath = "output_FarEastName.xlsx";
workbook.Save(outputPath);
// Reload to verify
Workbook verifyWorkbook = new Workbook(outputPath);
Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
}
}
}
```
### See Also
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
