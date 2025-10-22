##ShapeTextAlignment.Equals
ShapeTextAlignment method. Determines whether this instance has the same value as another specified ShapeTextAlignment object
## ShapeTextAlignment.Equals method
Determines whether this instance has the same value as another specified [`ShapeTextAlignment`](../) object.
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The [`ShapeTextAlignment`](../) object to compare with this instance. |
### Return Value
true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentMethodEqualsWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to compare text alignment
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
// Get another shape's text alignment for comparison
Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
ShapeTextAlignment obj = shape2.TextBody.TextAlignment;
if (shapeTextAlignment.Equals((object)obj))
{
Console.WriteLine("Text alignments are equal");
}
else
{
Console.WriteLine("Text alignments are not equal");
}
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
