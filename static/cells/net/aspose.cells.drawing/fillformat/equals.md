##FillFormat.Equals
FillFormat method.
## FillFormat.Equals method
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
using System.Drawing;
public class FillFormatMethodEqualsWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100); // Added width parameter
Shape shape2 = worksheet.Shapes.AddRectangle(0, 1, 0, 100, 100, 100); // Added width parameter
FillFormat fill1 = shape1.Fill;
FillFormat fill2 = shape2.Fill;
fill1.FillType = FillType.Solid;
fill1.SolidFill.Color = Color.Red;
fill2.FillType = FillType.Solid;
fill2.SolidFill.Color = Color.Red;
try
{
bool isEqual = fill1.Equals(fill2);
Console.WriteLine($"Fill formats are equal: {isEqual}");
fill2.SolidFill.Color = Color.Blue;
isEqual = fill1.Equals(fill2);
Console.WriteLine($"After modification, fill formats are equal: {isEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
workbook.Save("FillFormatEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
