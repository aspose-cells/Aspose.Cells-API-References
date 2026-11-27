---
title: "EquationNode.ToLaTeX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode method. Konvertera denna ekvation till ett LaTeX-uttryck"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Konvertera denna ekvation till LaTeX-uttryck.

```csharp
public string ToLaTeX()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Hämta ekvationsnoden
            var equationNode = shape.GetEquationParagraph();

            // Skapa en enkel bråkequation
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Anropa ToLaTeX-metoden
                string latexExpression = equationNode.ToLaTeX();
                
                // Visa resultatet
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Lägg till LaTeX-utdata i en cell
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


