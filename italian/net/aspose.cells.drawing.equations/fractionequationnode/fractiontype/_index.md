---
title: "FractionEquationNode.FractionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FractionEquationNode. Specifica il tipo di frazione; il valore predefinito è Bar"
type: docs
url: /it/net/aspose.cells.drawing.equations/fractionequationnode/fractiontype/
---
## FractionEquationNode.FractionType property

Questo specifica il tipo di frazione; il valore predefinito è 'Bar'.

```csharp
public EquationFractionType FractionType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FractionEquationNodePropertyFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni nodo matematico
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea nodo frazione
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
            string outputPath = "FractionEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Ricarica per verificare
            Workbook verifyWorkbook = new Workbook(outputPath);
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            FractionEquationNode verifyFraction = (FractionEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Fraction Type: " + verifyFraction.FractionType);
            Console.WriteLine("Numerator: " + ((TextRunEquationNode)verifyFraction.GetChild(0).GetChild(0)).Text);
            Console.WriteLine("Denominator: " + ((TextRunEquationNode)verifyFraction.GetChild(1).GetChild(0)).Text);
        }
    }
}
```

### Vedi anche

* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


