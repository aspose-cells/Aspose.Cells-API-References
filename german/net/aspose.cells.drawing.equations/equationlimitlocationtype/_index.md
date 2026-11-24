---
title: "Enum EquationLimitLocationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Gibt den Grenzort eines Operators an"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Gibt den Grenzwertort auf einem Operator an.

```csharp
public enum EquationLimitLocationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| UndOvr | `0` | Gibt an, dass die Grenze zentriert über oder unter dem Operator liegt. |
| SubSup | `1` | Gibt an, dass die Grenze sich auf der rechten Seite des Operators befindet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie dem Arbeitsblatt ein Gleichungs-Shape hinzu
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Rufen Sie den Gleichungsabsatz und dessen erstes Kind ab
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Erstellen Sie einen Nary-Gleichungsknoten
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Setzen Sie den Grenzort auf SubSup (rechte Seite des Operators)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Fügen Sie der Gleichung etwas Inhalt hinzu
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Ändern zu UndOvr (zentrierter über/unter Operator)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Speichere die Arbeitsmappe
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


