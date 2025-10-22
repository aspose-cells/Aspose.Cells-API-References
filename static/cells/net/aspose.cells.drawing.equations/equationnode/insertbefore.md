##EquationNode.InsertBefore
EquationNode method. Inserts the specified node before the current node
## EquationNode.InsertBefore method
Inserts the specified node before the current node.
```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types of Equation Nodes |
### Return Value
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a mathematical equation in cell A1
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
var equationNode = shape.GetEquationParagraph();
// Add initial text node to the equation
var textNode = equationNode.AddChild(EquationNodeType.Text);
textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary
try
{
// Insert a new text node before the existing one
var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary
Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
// Display the equation in LaTeX format
Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
}
catch (Exception ex)
{
Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
}
// Save the result
workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
