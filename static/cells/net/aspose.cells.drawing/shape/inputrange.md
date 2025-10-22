##Shape.InputRange
Shape property. Gets or sets the worksheet range used to fill the specified combo box
## Shape.InputRange property
Gets or sets the worksheet range used to fill the specified combo box.
```csharp
public string InputRange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyInputRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Value 1");
worksheet.Cells["A2"].PutValue("Value 2");
worksheet.Cells["A3"].PutValue("Value 3");
worksheet.Cells["A4"].PutValue("Value 4");
worksheet.Cells["A5"].PutValue("Value 5");
// Add a shape (rectangle)
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Set input range for the shape
shape.InputRange = "$A$1:$A$5";
// Check and modify input range if needed
if (shape.InputRange.Equals("$A$1:$A$5"))
{
shape.InputRange = "$B$1:$B$5";
Console.WriteLine("Input range changed to: " + shape.InputRange);
}
else
{
Console.WriteLine("Current input range: " + shape.InputRange);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
