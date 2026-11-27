---
title: "EquationNode.ParentNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode-egenskap. Anger föräldranoden för den aktuella noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Specificerar föräldranoden för den aktuella noden

```csharp
public EquationNode ParentNode { get; set; }
```

### Exempel

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
                // Skapa en textruta med ekvation
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Skapa en barnnod
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Visa värden för ParentNode-egenskapen
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Verifiera förälder-barn-relationen
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Visa hur man sätter ParentNode (eftersom den är läs‑skriv)
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

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


