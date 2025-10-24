##NaryEquationNode.LimitLocation
NaryEquationNode property. This attribute specifies the location of limits in nary operators. Limits can be either centered above and below the nary operator or positioned just to the right of the operator
## NaryEquationNode.LimitLocation property
This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator.
```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class NaryEquationNodePropertyLimitLocationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
// Access the equation and add a nary operator node
var equation = shape.GetEquationParagraph();
var naryNode = equation.AddChild(EquationNodeType.NaryEquation);
// Cast to NaryEquationNode to access LimitLocation
var naryEquationNode = (NaryEquationNode)naryNode;
try
{
// Display current LimitLocation (default value)
Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);
// Set LimitLocation to SubSup (limits on right side)
naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);
// Change back to UndOvr (centered limits)
naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);
// Save the workbook
workbook.Save("LimitLocationDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
