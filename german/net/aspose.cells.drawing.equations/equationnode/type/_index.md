---
title: "EquationNode.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Eigenschaft. Stellt den Typ des Knotens dar"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/type/
---
## EquationNode.Type property

Stellt den Typ des Knotens dar.

```csharp
public override TextNodeType Type { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform erstellen
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationRoot = shape.GetEquationParagraph();

            // Erstellen Sie verschiedene Typen von Gleichungsknoten
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Text";

            // Zeigen Sie die Type-Eigenschaft für verschiedene Knoten an
            Console.WriteLine($"Root equation node type: {equationRoot.Type}");
            Console.WriteLine($"Fraction node type: {fractionNode.Type}");
            Console.WriteLine($"Text node type: {textNode.Type}");

            // Erstellen Sie eine komplexe Gleichungsstruktur
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "Numerator";

            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "Denominator";

            // Prüfen Sie die Typen von Kindknoten
            Console.WriteLine($"Numerator node type: {numerator.Type}");
            Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
            Console.WriteLine($"Denominator node type: {denominator.Type}");

            // Demonstrieren Sie, wie Type das Verhalten von Knoten beeinflusst
            if (textNode.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("Text node is a TextRun type - can contain text content");
            }

            if (fractionNode.Type == TextNodeType.Equation)
            {
                Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
            }

            // Ergebnis speichern
            workbook.Save("EquationNodePropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


