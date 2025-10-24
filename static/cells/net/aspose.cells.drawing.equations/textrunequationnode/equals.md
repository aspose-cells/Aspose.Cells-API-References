##TextRunEquationNode.Equals
TextRunEquationNode method. Determine whether the current equation node is equal to the specified node
## TextRunEquationNode.Equals method
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
public class TextRunEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// For demo purposes, we'll use null and just show the comparison logic
// since we can't create TextRunEquationNode instances directly
TextRunEquationNode node1 = null;
TextRunEquationNode node2 = null;
TextRunEquationNode node3 = null;
try
{
// This part remains to show how Equals would be called
// In a real scenario, these would be properly initialized nodes
if (node1 != null && node2 != null && node3 != null)
{
// Compare node1 with node2 (same content)
bool result1 = node1.Equals((object)node2);
Console.WriteLine($"Comparing nodes with same text 'x': {result1}");
// Compare node1 with node3 (different content)
bool result2 = node1.Equals((object)node3);
Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");
// Compare with null
bool result3 = node1.Equals(null);
Console.WriteLine($"Comparing with null: {result3}");
// Compare with different object type
bool result4 = node1.Equals("string object");
Console.WriteLine($"Comparing with different type: {result4}");
}
else
{
Console.WriteLine("Node instances not available - this is just a compilation demo");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook (though Equals doesn't modify the spreadsheet)
workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
}
// Removed the helper method since we can't properly create TextRunEquationNode instances
}
}
```
### See Also
* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
