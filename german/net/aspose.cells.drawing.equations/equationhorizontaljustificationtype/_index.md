---
title: "Enum EquationHorizontalJustificationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. Dies gibt die standardmäßige horizontale Ausrichtung von Gleichungen im Dokument an"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

Dies gibt die standardmäßige horizontale Ausrichtung von Gleichungen im Dokument an.

```csharp
public enum EquationHorizontalJustificationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Center | `0` | Zentriert |
| CenterGroup | `1` | Zentriert als Gruppe |
| Left | `2` | Linksbündig |
| Right | `3` | Rechtsbündig |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie dem Arbeitsblatt ein Gleichungs-Shape hinzu
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Den Gleichungsabsatz abrufen
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // Verschiedene horizontale Ausrichtungstypen demonstrieren
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // Speichere die Arbeitsmappe
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


