---
title: EquationNode.ParentNode
second_title: Aspose.Cells for .NET API Reference
description: EquationNode property. Specifies the parent node of the current node
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Specifies the parent node of the current node

```csharp
public EquationNode ParentNode { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodePropertyParentNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a text box with equation
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Create a child node
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Display ParentNode property values
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Verify parent-child relationship
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Demonstrate setting ParentNode (since it's read-write)
                EquationNode newParent = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
                childNode.ParentNode = newParent;
                Console.WriteLine("After changing parent - Child's new parent: " + (childNode.ParentNode == newParent));

                workbook.Save("ParentNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


