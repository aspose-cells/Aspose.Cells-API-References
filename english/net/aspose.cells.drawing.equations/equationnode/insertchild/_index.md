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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an equation shape
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Add initial text node to the equation
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Insert a new fraction node at index 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Save the workbook
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


