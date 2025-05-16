---
title: EquationNode.InsertChild
second_title: Aspose.Cells for .NET API Reference
description: EquationNode method. Inserts a node of the specified type at the specified index position in the current nodes child node list
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Inserts a node of the specified type at the specified index position in the current node's child node list.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index value |
| equationType | EquationNodeType | Types of Equation Nodes |

### Return Value

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### Examples

```csharp
namespace AsposeCellsExamples.EquationNodeMethodInsertChildWithInt32EquationNodeTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a mathematical equation in cell A1
            var shape = worksheet.Shapes.AddTextBox(0, 0, 300, 50, 300, 50);
            var equation = shape.GetEquationParagraph();
            
            // Create a parent node (MathematicalEquation)
            var parentNode = equation.AddChild(EquationNodeType.MathematicalEquation);

            // Add initial child nodes to demonstrate insertion
            var initialNode = parentNode.AddChild(EquationNodeType.Text);
            initialNode.ToLaTeX(); // Workaround since Text property doesn't exist
            var textNode = parentNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround since Text property doesn't exist

            try
            {
                // Call InsertChild to insert a new Text node at index 1
                var insertedNode = parentNode.InsertChild(1, EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround since Text property doesn't exist

                Console.WriteLine("InsertChild method executed successfully with parameters (1, EquationNodeType.Text)");
                
                // Display the equation structure
                Console.WriteLine("Equation structure after insertion:");
                for (int i = 0; i < 3; i++) // Assuming we know there are 3 nodes now
                {
                    var child = parentNode.GetChild(i);
                    Console.WriteLine($"Node {i}: {child.ToLaTeX()}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("EquationNodeInsertChildDemo.xlsx");
        }
    }
}
```

### See Also

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


