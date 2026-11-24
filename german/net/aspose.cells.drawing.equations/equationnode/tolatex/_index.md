---
title: "EquationNode.ToLaTeX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Konvertiert diese Gleichung in einen LaTeX-Ausdruck"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Konvertiere diese Gleichung in einen LaTeX-Ausdruck.

```csharp
public string ToLaTeX()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um die Gleichung zu enthalten
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Den Gleichungsknoten abrufen
            var equationNode = shape.GetEquationParagraph();

            // Eine einfache Bruchgleichung erstellen
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Die ToLaTeX-Methode aufrufen
                string latexExpression = equationNode.ToLaTeX();
                
                // Ergebnis anzeigen
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Die LaTeX-Ausgabe zur Zelle hinzufügen
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


