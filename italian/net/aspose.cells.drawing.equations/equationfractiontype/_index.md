---
title: "Enum EquationFractionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Equations.EquationFractionType. Questo specifica lo stile di visualizzazione della barra di frazione"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Questo specifica lo stile di visualizzazione della barra di frazione.

```csharp
public enum EquationFractionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Bar | `0` | Questo specifica che il numeratore è sopra e il denominatore sotto, separati da una barra al centro. |
| NoBar | `1` | Questo specifica che il numeratore è sopra e il denominatore sotto, ma non sono separati da una barra al centro. |
| Linear | `2` | Questo specifica che il numeratore è a sinistra e il denominatore è a destra, separati da un '/' al centro. |
| Skewed | `3` | Questo specifica che il numeratore è in alto a sinistra e il denominatore è in basso a destra, separati da un \"/\". |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo matematico e aggiungi la frazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Aggiungi numeratore
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Aggiungi denominatore
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Salva e verifica
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


