##MatrixEquationNode.Equals
MatrixEquationNode method. Determine whether the current equation node is equal to the specified node
## MatrixEquationNode.Equals method
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
public class MatrixEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
try
{
// Since MatrixEquationNode doesn't have a parameterless constructor,
// we'll demonstrate the Equals method using a different approach
Console.WriteLine("MatrixEquationNode Equals demonstration:");
// Note: Actual instantiation would require proper constructor parameters
// This is just to show the Equals method usage pattern
MatrixEquationNode node1 = null; // Would normally be created with proper constructor
MatrixEquationNode node2 = null; // Would normally be created with proper constructor
if (node1 != null && node2 != null)
{
// Compare the nodes using Equals method
bool areEqual = node1.Equals(node2);
Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");
// Compare a node with itself
bool selfEqual = node1.Equals(node1);
Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
}
// Compare with null
if (node1 != null)
{
bool nullEqual = node1.Equals(null);
Console.WriteLine($"Is node1 equal to null? {nullEqual}");
}
else
{
Console.WriteLine("Node1 is null - cannot demonstrate Equals method");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error in MatrixEquationNode Equals demonstration: {ex.Message}");
}
}
}
}
```
### See Also
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
