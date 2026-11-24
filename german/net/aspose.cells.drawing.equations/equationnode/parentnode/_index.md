---
title: "EquationNode.ParentNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Eigenschaft. Gibt den übergeordneten Knoten des aktuellen Knotens an"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Gibt den übergeordneten Knoten des aktuellen Knotens an

```csharp
public EquationNode ParentNode { get; set; }
```

### Beispiele

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
                // Erstellen Sie ein Textfeld mit Gleichung
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Erstellen Sie einen Kindknoten
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Zeigen Sie die Werte der ParentNode-Eigenschaft an
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Überprüfen Sie die Eltern-Kind-Beziehung
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Demonstrieren Sie das Setzen von ParentNode (da es les- und schreibbar ist)
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

### Siehe auch

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


