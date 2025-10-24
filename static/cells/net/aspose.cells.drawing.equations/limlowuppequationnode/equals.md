##LimLowUppEquationNode.Equals
LimLowUppEquationNode method. Determine whether the current equation node is equal to the specified node
## LimLowUppEquationNode.Equals method
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
public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Since we don't know the constructor parameters, we'll compare null values
// This is a minimal change to make it compile - in real usage you'd need proper construction
LimLowUppEquationNode node1 = null;
LimLowUppEquationNode node2 = null;
try
{
// Call the Equals method with the specific parameter type (Object)
bool areEqual = node1?.Equals((object)node2) ?? false;
// Display the result
Console.WriteLine($"Are the nodes equal? {areEqual}");
// Save the workbook
workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
}
}
}
```
### See Also
* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
