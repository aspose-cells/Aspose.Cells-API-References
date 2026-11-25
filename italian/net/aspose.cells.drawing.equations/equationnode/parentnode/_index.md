---
title: "EquationNode.ParentNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà EquationNode. Specifica il nodo genitore del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Specifica il nodo genitore del nodo corrente

```csharp
public EquationNode ParentNode { get; set; }
```

### Esempi

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
                // Crea una casella di testo con equazione
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Crea un nodo figlio
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Visualizza i valori della proprietà ParentNode
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Verifica la relazione genitore-figlio
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Dimostra l'impostazione di ParentNode (poiché è leggibile-scrivibile)
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

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


