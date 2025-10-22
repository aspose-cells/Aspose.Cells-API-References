##ArrayEquationNode.Equals
ArrayEquationNode method. Determine whether the current equation node is equal to the specified node
## ArrayEquationNode.Equals method
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
public class ArrayEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two array equation nodes
ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
// Add child nodes to make them different
EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
// Use ToLaTeX() or ToMathML() instead of Value property
arrayEquation1.AddChild(child1);
EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
arrayEquation2.AddChild(child2);
try
{
// Call Equals method with different objects
bool result1 = arrayEquation1.Equals(arrayEquation2);
Console.WriteLine($"Comparing different array equations: {result1}");
// Call Equals with same object
bool result2 = arrayEquation1.Equals(arrayEquation1);
Console.WriteLine($"Comparing same array equation: {result2}");
// Call Equals with null
bool result4 = arrayEquation1.Equals(null);
Console.WriteLine($"Comparing with null: {result4}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
