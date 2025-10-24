##SolidFill.Equals
SolidFill method.
## SolidFill.Equals method
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
public class SolidFillMethodEqualsWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape1 = worksheet.Shapes.AddRectangle(3, 0, 3, 0, 200, 200);
Shape shape2 = worksheet.Shapes.AddRectangle(3, 0, 3, 0, 200, 200);
try
{
FillFormat fill1 = shape1.Fill;
fill1.FillType = FillType.Solid;
SolidFill solidFill1 = fill1.SolidFill;
solidFill1.Color = Color.Red;
solidFill1.Transparency = 0.2;
FillFormat fill2 = shape2.Fill;
fill2.FillType = FillType.Solid;
SolidFill solidFill2 = fill2.SolidFill;
solidFill2.Color = Color.Red;
solidFill2.Transparency = 0.2;
bool areEqual = solidFill1.Equals((object)solidFill2);
Console.WriteLine($"SolidFill objects are equal: {areEqual}");
solidFill2.Color = Color.Blue;
areEqual = solidFill1.Equals((object)solidFill2);
Console.WriteLine($"After modification, SolidFill objects are equal: {areEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
workbook.Save("SolidFillEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
