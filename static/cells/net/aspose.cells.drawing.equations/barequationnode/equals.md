##BarEquationNode.Equals
BarEquationNode method. Determine whether the current equation node is equal to the specified node
## BarEquationNode.Equals method
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
public class BarEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two BarEquationNode instances for comparison
// Note: Actual creation of BarEquationNode would depend on API's factory methods
// For demonstration, we'll assume these are properly initialized instances
BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);
try
{
// Compare node1 with node2 (should be equal)
bool result1 = node1.Equals(node2);
Console.WriteLine($"Comparing node1 with node2: {result1}");
// Compare node1 with node3 (should not be equal)
bool result2 = node1.Equals(node3);
Console.WriteLine($"Comparing node1 with node3: {result2}");
// Compare node1 with null
bool result3 = node1.Equals(null);
Console.WriteLine($"Comparing node1 with null: {result3}");
// Compare node1 with a different object type
bool result4 = node1.Equals("string object");
Console.WriteLine($"Comparing node1 with string: {result4}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("BarEquationNodeEqualsDemo.xlsx");
}
// Helper method to demonstrate getting a BarEquationNode
// In real usage, you would use the proper API method to create these
private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
{
// This is just a placeholder - actual implementation would depend on the API
// For example, it might be created through a parent object or factory method
return null; // Replace with actual creation code
}
}
}
```
### See Also
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
