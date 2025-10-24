##MathematicalEquationNode.Equals
MathematicalEquationNode method. Determine whether the current equation node is equal to the specified node
## MathematicalEquationNode.Equals method
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
using Aspose.Cells.Drawing.Equations;
using System;
public class MathematicalEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
try
{
// Create two MathematicalEquationNode instances for comparison
// Since MathematicalEquationNode doesn't have a parameterless constructor,
// we'll need to pass null or appropriate parameters
MathematicalEquationNode node1 = null;
MathematicalEquationNode node2 = null;
// Compare the nodes using Equals method
bool areEqual = node1?.Equals((object)node2) ?? false;
// Display the comparison result
Console.WriteLine($"Nodes are equal: {areEqual}");
// Compare with a different object type
object differentObject = new object();
bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
}
catch (Exception ex)
{
Console.WriteLine($"Error in Equals comparison: {ex.Message}");
}
}
}
}
```
### See Also
* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
