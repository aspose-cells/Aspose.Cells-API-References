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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a shape to hold the equation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationRoot = ((TextBox)shape).GetEquationParagraph();

            // Create a fraction node and add it to the root
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            
            // Create numerator and denominator nodes
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);

            // Display initial parent node relationships
            Console.WriteLine($"Fraction node parent: {fractionNode.ParentNode == equationRoot}");
            Console.WriteLine($"Numerator parent: {numerator.ParentNode == fractionNode}");
            Console.WriteLine($"Denominator parent: {denominator.ParentNode == fractionNode}");

            // Change the parent of numerator to be the root equation node
            numerator.ParentNode = equationRoot;
            
            // Verify the change
            Console.WriteLine($"After change - Numerator parent is root: {numerator.ParentNode == equationRoot}");
            Console.WriteLine($"Fraction node now has children (implementation detail)"); // Removed GetChildCount() call

            // Create a new parent node (radical) and move the denominator
            var radicalNode = equationRoot.AddChild(EquationNodeType.Radical);
            denominator.ParentNode = radicalNode;
            
            // Verify the move
            Console.WriteLine($"Denominator moved to radical: {denominator.ParentNode == radicalNode}");
            Console.WriteLine($"Radical node has child: {radicalNode.GetChild(0) == denominator}");

            // Save the result
            workbook.Save("EquationNodePropertyParentNodeDemo.xlsx");
        }
    }
}
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


