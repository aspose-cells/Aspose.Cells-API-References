---
title: "EquationNode.ToLaTeX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Converte questa equazione in espressione LaTeX"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Converti questa equazione in espressione LaTeX.

```csharp
public string ToLaTeX()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per contenere l'equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Ottieni il nodo dell'equazione
            var equationNode = shape.GetEquationParagraph();

            // Crea un'equazione di frazione semplice
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Chiama il metodo ToLaTeX
                string latexExpression = equationNode.ToLaTeX();
                
                // Visualizza il risultato
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Aggiungi l'output LaTeX a una cella
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


