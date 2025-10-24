##EquationNode.Equals
EquationNode method. Determine whether the current equation node is equal to the specified node
## EquationNode.Equals method
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
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two equation nodes for comparison
EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
try
{
// Call Equals method with Object parameter
bool areEqual = node1.Equals((object)node2);
Console.WriteLine($"Are the equation nodes equal? {areEqual}");
// Modify node2 to make them different
node2.AddChild(EquationNodeType.Base);
areEqual = node1.Equals((object)node2);
Console.WriteLine($"After modification, are they equal? {areEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
workbook.Save("EquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
