##Shape.MacroName
Shape property. Gets and sets the name of macro
## Shape.MacroName property
Gets and sets the name of macro.
```csharp
public string MacroName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyMacroNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Set the macro name for the shape
shape.MacroName = "DoWork()";
// Output confirmation
Console.WriteLine("Shape macro name set to: " + shape.MacroName);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
