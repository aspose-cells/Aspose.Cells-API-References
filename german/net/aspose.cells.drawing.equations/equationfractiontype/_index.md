---
title: "Enum EquationFractionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationFractionType enum. Dies gibt den Anzeigestil des Bruchstrichs an"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Dies gibt den Anzeigestil des Bruchstrichs an.

```csharp
public enum EquationFractionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Bar | `0` | Dies gibt an, dass der Zähler oben und der Nenner unten durch einen Strich in der Mitte getrennt sind. |
| NoBar | `1` | Dies gibt an, dass der Zähler oben und der Nenner unten nicht durch einen Strich in der Mitte getrennt sind. |
| Linear | `2` | Dies gibt an, dass der Zähler links und der Nenner rechts steht, getrennt durch ein '/' dazwischen. |
| Skewed | `3` | Dies gibt an, dass der Zähler oben links und der Nenner unten rechts steht, getrennt durch ein \"/\". |

### Beispiele

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
            
            // Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hole den Mathematik-Knoten und füge einen Bruch hinzu
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
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
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


