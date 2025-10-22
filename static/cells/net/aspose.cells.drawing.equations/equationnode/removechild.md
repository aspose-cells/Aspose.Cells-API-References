##EquationNode.RemoveChild
EquationNode method. Removes the specified node from the current nodes children
## RemoveChild(EquationNode) {#removechild}
Removes the specified node from the current node's children.
```csharp
public void RemoveChild(EquationNode node)
```
| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | Node to be deleted. |
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
## RemoveChild(int) {#removechild_1}
Removes the node at the specified index from the current node's children.
```csharp
public void RemoveChild(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Index of the node |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Equations;
using System;
public class EquationNodeMethodRemoveChildWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a parent equation node
EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
// Add child nodes
EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);
try
{
// Remove child at index 1 (second child)
parentNode.RemoveChild(1);
Console.WriteLine("Child at index 1 removed successfully");
// Verify removal by checking remaining children
EquationNode remainingChild = parentNode.GetChild(0);
Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
// Attempt to get removed child (should throw)
try
{
var removedChild = parentNode.GetChild(1);
}
catch (Exception ex)
{
Console.WriteLine($"Expected error when accessing removed child: {ex.Message}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveChild method: {ex.Message}");
}
workbook.Save("EquationNodeRemoveChildWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
