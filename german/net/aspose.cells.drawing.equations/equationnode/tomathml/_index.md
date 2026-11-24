---
title: "EquationNode.ToMathML"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Konvertiere diese Gleichung in einen MathML-Ausdruck"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

Konvertiere diese Gleichung in einen MathML-Ausdruck.

```csharp
public string ToMathML()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToMathMLDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Gleichungs-Shape - hinzugefügter Breitenparameter (300) und Höhenparameter (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // Erstelle eine einfache Gleichung: (a+b)^2 = a^2 + 2ab + b^2
            var equationNode = equation.AddChild(EquationNodeType.Text);
            var textNode = equationNode as TextRunEquationNode;
            textNode.Text = "(";

            var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableA.Text = "a";

            var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            plus.Text = "+";

            var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableB.Text = "b";

            var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            closeParen.Text = ")";

            var superscript = equation.AddChild(EquationNodeType.Superscript);
            var baseNode = superscript.AddChild(EquationNodeType.Base);
            var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            baseText.Text = "2";

            try
            {
                // Konvertiere die Gleichung in MathML
                string mathML = equation.ToMathML();

                // Gib das MathML in der Konsole aus
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // Schreibe das MathML in eine Zelle
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // Geändert von worksheet.Cells.AutoFitColumns() zu:
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


