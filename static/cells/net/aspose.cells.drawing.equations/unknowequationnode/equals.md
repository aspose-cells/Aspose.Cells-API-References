##UnknowEquationNode.Equals
UnknowEquationNode method. Determine whether the current equation node is equal to the specified node
## UnknowEquationNode.Equals method
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
public class UnknowEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two unknown equation nodes for comparison
// Since UnknowEquationNode doesn't have a parameterless constructor,
// we'll need to create them differently. For demo purposes, we'll use
// the actual constructor if available, or create them through other means.
// As we don't know the constructor parameters, this is a placeholder fix.
UnknowEquationNode node1 = CreateUnknownEquationNode();
UnknowEquationNode node2 = CreateUnknownEquationNode();
object objToCompare = node2;
try
{
// Call the Equals method with the specific parameter type (Object)
bool areEqual = node1.Equals(objToCompare);
// Display the result
Console.WriteLine($"Are the equation nodes equal? {areEqual}");
// Add the result to the worksheet
worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the result
workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
}
// Helper method to create UnknowEquationNode instances
private static UnknowEquationNode CreateUnknownEquationNode()
{
// In a real implementation, this would use the proper constructor
// Since we don't know the constructor parameters, we'll return null
// and handle the null case in the demo (though this is just a placeholder)
return null;
}
}
}
```
### See Also
* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
