##EquationNode.InsertAfter
EquationNode method. Inserts the specified node after the current node
## EquationNode.InsertAfter method
Inserts the specified node after the current node.
```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
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
public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an equation shape in cell A1
var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
var equationNode = shape.GetEquationParagraph();
// Add initial text node
var firstNode = equationNode.AddChild(EquationNodeType.Text);
if (firstNode is TextRunEquationNode textNode)
{
textNode.Text = "Initial Text";
}
try
{
// Insert a new text node after the existing one
var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
if (insertedNode is TextRunEquationNode insertedTextNode)
{
insertedTextNode.Text = "Inserted After";
}
Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
// Display the equation structure
Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
// Save the equation to a cell for visual inspection
worksheet.Cells["A2"].PutValue("Equation Output:");
worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
}
catch (Exception ex)
{
Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
}
// Save the workbook
workbook.Save("EquationNodeInsertAfterDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
