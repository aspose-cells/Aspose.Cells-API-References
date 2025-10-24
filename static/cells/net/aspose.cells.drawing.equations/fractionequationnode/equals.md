##FractionEquationNode.Equals
FractionEquationNode method. Determine whether the current equation node is equal to the specified node
## FractionEquationNode.Equals method
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
public class FractionEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
try
{
// Since FractionEquationNode doesn't have a parameterless constructor,
// we'll demonstrate Equals with objects that would presumably come from elsewhere in the API
// For demonstration purposes, we'll assume we have two instances to compare
FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);
// Compare the objects using Equals
bool areEqual = node1.Equals(node2);
// Display the comparison result
Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");
// Compare with null
bool isNullEqual = node1.Equals(null);
Console.WriteLine($"Comparison with null: {isNullEqual}");
// Compare with self
bool isSelfEqual = node1.Equals(node1);
Console.WriteLine($"Comparison with self: {isSelfEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
}
}
// Helper method to simulate getting FractionEquationNode instances
// (In real usage, these would come from the API)
private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
{
// This is just a placeholder - in reality you would get these from the API
// For example: worksheet.Equations.AddFractionEquationNode() or similar
return null; // Actual implementation would depend on API
}
}
}
```
### See Also
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
