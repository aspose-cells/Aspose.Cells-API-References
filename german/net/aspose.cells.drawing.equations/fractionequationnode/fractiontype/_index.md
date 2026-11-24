---
title: "FractionEquationNode.FractionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FractionEquationNode-Eigenschaft. Gibt den Typ des Bruchs an, standardmäßig ist Bar"
type: docs
url: /de/net/aspose.cells.drawing.equations/fractionequationnode/fractiontype/
---
## FractionEquationNode.FractionType property

Dies gibt den Typ des Bruchs an; standardmäßig ist 'Bar'.

```csharp
public EquationFractionType FractionType { get; set; }
```

### Beispiele

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
            
            // Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Math-Knoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bruchknoten erstellen
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Zähler hinzufügen
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Nenner hinzufügen
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Speichern und überprüfen
            string outputPath = "FractionEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Neu laden, um zu überprüfen
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

### Siehe auch

* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


