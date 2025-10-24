##EquationNodeParagraph.Equals
EquationNodeParagraph method. Determine whether the current equation node is equal to the specified node
## EquationNodeParagraph.Equals method
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
public class EquationNodeParagraphMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two EquationNodeParagraph instances for comparison
// Using the CreateNode method to properly instantiate the nodes
EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
// Set different justification types to make them unequal
paragraph1.Justification = EquationHorizontalJustificationType.Center;
paragraph2.Justification = EquationHorizontalJustificationType.Left;
try
{
// Call the Equals method with paragraph2 as the parameter
bool areEqual = paragraph1.Equals(paragraph2);
// Display the comparison result
Console.WriteLine($"Are the paragraphs equal? {areEqual}");
// Create another paragraph with same justification as paragraph1
EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
paragraph3.Justification = EquationHorizontalJustificationType.Center;
// Call Equals again with paragraph3
areEqual = paragraph1.Equals(paragraph3);
Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");
// Also demonstrate comparison with null
areEqual = paragraph1.Equals(null);
Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook (though no visible changes were made to the worksheet)
workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
