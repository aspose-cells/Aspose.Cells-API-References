##Shape.Spid
Shape property. Specifies an optional string identifier that an application can use to identify the particular shape
## Shape.Spid property
Specifies an optional string identifier that an application can use to identify the particular shape.
```csharp
public string Spid { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertySpidDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);
// Get and display the Spid property of the shape
string spid = shape.Spid;
Console.WriteLine("Shape SPID: " + spid);
// Save the workbook
workbook.Save("ShapePropertySpidDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
