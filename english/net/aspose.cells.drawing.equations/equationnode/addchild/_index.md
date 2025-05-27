---
title: EquationNode.AddChild
second_title: Aspose.Cells for .NET API Reference
description: EquationNode method. Insert a node of the specified type at the end of the child node list of the current node
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/addchild/
---
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

---

## AddChild(EquationNode) {#addchild_1}

Inserts the specified node at the end of the current node's list of child nodes.

```csharp
public void AddChild(EquationNode node)
```

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | The specified node |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an equation shape
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // Create parent node (fraction)
            var fractionNode = equation.AddChild(EquationNodeType.Fraction);

            // Create child node (numerator)
            var numeratorNode = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numeratorNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "x";

            // Create another node to add as child (denominator)
            var denominatorNode = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominatorNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "y";

            try
            {
                Console.WriteLine("Equation structure after AddChild:");
                Console.WriteLine(equation.ToMathML());

                // Display equation in a cell
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["A2"].PutValue(equation.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddChild method: {ex.Message}");
            }

            // Save the result
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


