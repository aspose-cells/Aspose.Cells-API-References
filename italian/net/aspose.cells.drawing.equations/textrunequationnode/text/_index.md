---
title: "TextRunEquationNode.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextRunEquationNode. Imposta il contenuto del nodo di testo, solitamente un oggetto nodo per carattere"
type: docs
url: /it/net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Imposta il contenuto del nodo di testo (di solito un oggetto nodo per carattere).

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextRunEquationNodePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo radice dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un'equazione frazionaria
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Aggiungi il numeratore con il testo "X"
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Aggiungi il denominatore con il testo "Y"
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Salva la cartella di lavoro
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            // Verifica il file salvato ricaricandolo
            Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Accedi alle proprietà del testo per dimostrare la funzionalità
            TextRunEquationNode loadedNumeratorText = (TextRunEquationNode)((FractionEquationNode)loadedTextBox
                .GetEquationParagraph()
                .GetChild(0)
                .GetChild(0))
                .GetChild(0)
                .GetChild(0);

            Console.WriteLine("Numerator text: " + loadedNumeratorText.Text);
        }
    }
}
```

### Vedi anche

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


