##EquationNode.CreateNode
EquationNode method. Create a node of the specified type
## EquationNode.CreateNode method
Create a node of the specified type.
```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook,
EquationNode parent)
```
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types of Equation Nodes |
| workbook | Workbook | The workbook object associated with the equation |
| parent | EquationNode | The parent node where this node is located |
### Return Value
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an equation shape
var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
var equationNode = shape.GetEquationParagraph();
try
{
// Create a parent node (fraction)
var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
// Create numerator and denominator nodes
var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
numeratorText.Text = "a + b";
var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
denominatorText.Text = "c";
// Add the created fraction to the main equation
equationNode.AddChild(fractionNode);
Console.WriteLine("Equation created successfully using CreateNode method");
// Display equation in a cell
worksheet.Cells["A1"].PutValue("Equation Output:");
worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
worksheet.AutoFitColumns();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
}
// Save the result
workbook.Save("EquationNodeCreateNodeDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
