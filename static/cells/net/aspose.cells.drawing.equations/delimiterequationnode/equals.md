##DelimiterEquationNode.Equals
DelimiterEquationNode method. Determine whether the current equation node is equal to the specified node
## DelimiterEquationNode.Equals method
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
public class DelimiterEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two DelimiterEquationNode instances for comparison
// Since DelimiterEquationNode doesn't have a parameterless constructor,
// we'll need to create them differently. Assuming we can use the default constructor
// of the base class or find another way to create them.
// For demonstration, we'll use ObjectCreationHelper (hypothetical) or similar approach
DelimiterEquationNode node1 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
node1.BeginChar = "(";
node1.EndChar = ")";
node1.SeparatorChar = ",";
node1.DelimiterShape = EquationDelimiterShapeType.Centered;
DelimiterEquationNode node2 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
node2.BeginChar = "(";
node2.EndChar = ")";
node2.SeparatorChar = ",";
node2.DelimiterShape = EquationDelimiterShapeType.Centered;
try
{
// Call the Equals method with Object parameter
bool result = node1.Equals((Object)node2);
// Display the result
Console.WriteLine($"Equals method result: {result}");
// Modify node2 to make them different
node2.BeginChar = "[";
bool result2 = node1.Equals((Object)node2);
Console.WriteLine($"Equals method result after modification: {result2}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
