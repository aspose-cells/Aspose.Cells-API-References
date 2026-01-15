---
title: FunctionEquationNode.Equals
second_title: Aspose.Cells for .NET API Reference
description: FunctionEquationNode method. Determine whether the current equation node is equal to the specified node
type: docs
url: /net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Determine whether the current equation node is equal to the specified node

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a TextBox shape to hold an equation
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Get the root equation node of the TextBox
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Create the first function equation node
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Optional) Add minimal content to make the node valid
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Create the second function equation node
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Compare the two function nodes using Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Compare a node to itself
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Save the workbook (no visual changes needed for this demo)
                workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


