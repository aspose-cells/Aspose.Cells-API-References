##Shape.IsWordArt
Shape property. Indicates whether this shape is a word art
## Shape.IsWordArt property
Indicates whether this shape is a word art.
```csharp
public bool IsWordArt { get; }
```
### Remarks
Only for the Legacy Shape of xls file.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsWordArtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a WordArt shape with all required parameters
Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);
// Add a regular rectangle shape with all required parameters
Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);
// Check if shapes are WordArt
Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);
// Example usage of IsWordArt property
if (wordArt.IsWordArt)
{
Console.WriteLine("First shape is a WordArt object");
}
if (!rectangle.IsWordArt)
{
Console.WriteLine("Second shape is not a WordArt object");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
