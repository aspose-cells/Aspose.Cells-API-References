##ThreeDFormat.Equals
ThreeDFormat method.
## ThreeDFormat.Equals method
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to compare 3D formats
Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);
// Get the 3D formats of the shapes
ThreeDFormat format1 = shape1.ThreeDFormat;
ThreeDFormat format2 = shape2.ThreeDFormat;
// Configure identical 3D settings
format1.BottomBevelWidth = 10;
format1.BottomBevelHeight = 10;
format1.BottomBevelType = BevelType.ArtDeco;
format2.BottomBevelWidth = 10;
format2.BottomBevelHeight = 10;
format2.BottomBevelType = BevelType.ArtDeco;
try
{
// Call the Equals method to compare the 3D formats
bool areEqual = format1.Equals((object)format2);
// Display the result
Console.WriteLine($"The 3D formats are equal: {areEqual}");
// Modify one property to make them different
format2.BottomBevelWidth = 15;
areEqual = format1.Equals((object)format2);
Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("ThreeDFormatEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
