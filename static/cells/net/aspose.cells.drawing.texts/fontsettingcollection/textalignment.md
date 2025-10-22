##FontSettingCollection.TextAlignment
FontSettingCollection property. Represents the alignment setting of the text body
## FontSettingCollection.TextAlignment property
Represents the alignment setting of the text body.
```csharp
public ShapeTextAlignment TextAlignment { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FontSettingCollectionPropertyTextAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
shape.Text = "Sample Text";
// Access and modify TextAlignment properties
var textAlignment = shape.TextBody.TextAlignment;
Console.WriteLine("Default Margins (Points):");
Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
// Modify margins
textAlignment.TopMarginPt = 36;
textAlignment.BottomMarginPt = 36;
textAlignment.LeftMarginPt = 18;
textAlignment.RightMarginPt = 18;
// Save the workbook
workbook.Save("TextAlignmentDemo.xlsx");
Console.WriteLine("\nModified Margins (Points):");
Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
