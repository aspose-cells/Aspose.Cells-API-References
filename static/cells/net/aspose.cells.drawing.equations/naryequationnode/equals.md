##NaryEquationNode.Equals
NaryEquationNode method. Determine whether the current equation node is equal to the specified node
## NaryEquationNode.Equals method
Determine whether the current equation node is equal to the specified node
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
using System;
public class NaryEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to hold the equation
var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
var equation1 = shape1.GetEquationParagraph();
var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
var naryEquationNode1 = (NaryEquationNode)naryNode1;
naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;
// Create a second identical shape
var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
var equation2 = shape2.GetEquationParagraph();
var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
var naryEquationNode2 = (NaryEquationNode)naryNode2;
naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;
// Create a third different shape
var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
var equation3 = shape3.GetEquationParagraph();
var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
var naryEquationNode3 = (NaryEquationNode)naryNode3;
naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;
try
{
// Compare identical nodes
bool result1 = naryEquationNode1.Equals(naryEquationNode2);
Console.WriteLine($"Comparing identical nodes: {result1}");
// Compare different nodes
bool result2 = naryEquationNode1.Equals(naryEquationNode3);
Console.WriteLine($"Comparing different nodes: {result2}");
// Compare with null
bool result3 = naryEquationNode1.Equals(null);
Console.WriteLine($"Comparing with null: {result3}");
// Compare with different object type
bool result4 = naryEquationNode1.Equals("string object");
Console.WriteLine($"Comparing with different type: {result4}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
