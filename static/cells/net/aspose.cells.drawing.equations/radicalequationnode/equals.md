##RadicalEquationNode.Equals
RadicalEquationNode method. Determine whether the current equation node is equal to the specified node
## RadicalEquationNode.Equals method
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
public class RadicalEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
try
{
// Create two RadicalEquationNode instances
RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
// Set different properties to demonstrate equality comparison
node1.IsDegHide = true;
node2.IsDegHide = false;
// Compare the nodes using Equals method
bool areEqual = node1.Equals(node2);
// Display the comparison result
Console.WriteLine($"Are nodes equal? {areEqual}");
// Compare with the same object
areEqual = node1.Equals(node1);
Console.WriteLine($"Are node1 and itself equal? {areEqual}");
// Compare with null
areEqual = node1.Equals(null);
Console.WriteLine($"Are node1 and null equal? {areEqual}");
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
* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
