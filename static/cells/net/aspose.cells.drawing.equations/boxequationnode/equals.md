##BoxEquationNode.Equals
BoxEquationNode method. Determine whether the current equation node is equal to the specified node
## BoxEquationNode.Equals method
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
public class BoxEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two BoxEquationNode objects for comparison
// Since BoxEquationNode doesn't have a parameterless constructor,
// we'll need to create them differently. Assuming we can get them from somewhere,
// or create them with some default parameters.
// For demo purposes, we'll just declare them and assign null (though in real code you'd need proper initialization)
BoxEquationNode node1 = null;
BoxEquationNode node2 = null;
object objToCompare = node2;
try
{
if (node1 != null && node2 != null)
{
// Call the Equals method with the specific parameter types (Object)
bool areEqual = node1.Equals(objToCompare);
// Display the result
Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");
// Add the result to the worksheet
worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
worksheet.Cells["B1"].PutValue(areEqual);
}
else
{
Console.WriteLine("BoxEquationNode objects not properly initialized");
worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
worksheet.Cells["A1"].PutValue("Error occurred:");
worksheet.Cells["B1"].PutValue(ex.Message);
}
// Save the result
workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
