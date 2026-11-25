---
title: "EquationNode.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà EquationNode. Rappresenta il tipo del nodo"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/type/
---
## EquationNode.Type property

Rappresenta il tipo del nodo.

```csharp
public override TextNodeType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class EquationNodePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationRoot = shape.GetEquationParagraph();

            // Crea diversi tipi di nodi di equazione
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Text";

            // Visualizza la proprietà Type per diversi nodi
            Console.WriteLine($"Root equation node type: {equationRoot.Type}");
            Console.WriteLine($"Fraction node type: {fractionNode.Type}");
            Console.WriteLine($"Text node type: {textNode.Type}");

            // Crea una struttura di equazione complessa
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "Numerator";

            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "Denominator";

            // Verifica i tipi dei nodi figlio
            Console.WriteLine($"Numerator node type: {numerator.Type}");
            Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
            Console.WriteLine($"Denominator node type: {denominator.Type}");

            // Dimostra come Type influisce sul comportamento del nodo
            if (textNode.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("Text node is a TextRun type - can contain text content");
            }

            if (fractionNode.Type == TextNodeType.Equation)
            {
                Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
            }

            // Salva il risultato
            workbook.Save("EquationNodePropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


