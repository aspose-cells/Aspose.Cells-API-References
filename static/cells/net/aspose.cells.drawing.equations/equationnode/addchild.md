##EquationNode.AddChild
EquationNode method. Insert a node of the specified type at the end of the child node list of the current node
## AddChild(EquationNodeType) {#addchild}
Insert a node of the specified type at the end of the child node list of the current node.
```csharp
public EquationNode AddChild(EquationNodeType equationType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types of Equation Nodes |
### Return Value
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;
namespace AsposeCellsExamples
{
public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add an equation shape to the first worksheet
TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
// Get the root math node
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
// Create a function node and add children
FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
// Add function name with superscript
EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
// Add base text for function name
EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
baseText.Text = "Add";
// Add superscript text
EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
superscriptText.Text = "-2";
// Add function argument
EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
argumentText.Text = "x";
// Save the workbook
workbook.Save("EquationNodeAddChildDemo.xlsx");
}
}
}
```
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
## AddChild(EquationNode) {#addchild_1}
Inserts the specified node at the end of the current node's list of child nodes.
```csharp
public void AddChild(EquationNode node)
```
| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | The specified node |
### See Also
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
