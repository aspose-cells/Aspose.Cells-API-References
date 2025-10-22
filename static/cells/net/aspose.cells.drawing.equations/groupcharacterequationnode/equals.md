##GroupCharacterEquationNode.Equals
GroupCharacterEquationNode method. Determine whether the current equation node is equal to the specified node
## GroupCharacterEquationNode.Equals method
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
public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two GroupCharacterEquationNode instances for comparison
// Since GroupCharacterEquationNode doesn't have a parameterless constructor,
// we'll need to create them through the worksheet's ShapeCollection
var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
node1.GroupChr = "⏟";
node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
node1.Position = EquationCharacterPositionType.Bottom;
node1.VertJc = EquationCharacterPositionType.Bottom;
var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
node2.GroupChr = "⏟";
node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
node2.Position = EquationCharacterPositionType.Bottom;
node2.VertJc = EquationCharacterPositionType.Bottom;
try
{
// Call the Equals method with Object parameter
bool areEqual = node1.Equals((Object)node2);
// Display the comparison result
Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");
// Add the result to the worksheet
worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
worksheet.Cells["A2"].PutValue(areEqual);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the result
workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
