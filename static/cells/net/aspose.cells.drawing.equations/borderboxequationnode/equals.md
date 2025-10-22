##BorderBoxEquationNode.Equals
BorderBoxEquationNode method. Determine whether the current equation node is equal to the specified node
## BorderBoxEquationNode.Equals method
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
public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
try
{
// Create two BorderBoxEquationNode instances for comparison
// Since BorderBoxEquationNode doesn't have a parameterless constructor,
// we'll use the base class constructor (assuming EquationNode might have one)
BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
// Compare the nodes using Equals method
bool areEqual = node1.Equals((object)node2);
// Display the comparison result
Console.WriteLine($"The nodes are equal: {areEqual}");
// Compare with a different object type
object differentObject = new object();
bool areEqualWithDifferentType = node1.Equals(differentObject);
Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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
* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
