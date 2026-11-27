---
title: "Enum EquationLimitLocationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType‑enum. Anger gränsens placering på en operator"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Specificerar gränsplatsen på en operator.

```csharp
public enum EquationLimitLocationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| UndOvr | `0` | Anger att gränsen är centrerad ovanför eller nedanför operatorn. |
| SubSup | `1` | Anger att gränsen är på höger sida av operatorn. |

### Exempel

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
                // Lägg till en ekvationsform till kalkylbladet
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Hämta ekvations‑paragrafen och dess första barn
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Skapa en Nary‑ekvationsnod
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Ställ in gränsens placering till SubSup (höger sida av operatorn)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Lägg till lite innehåll i ekvationen
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Ändra till UndOvr (centrerad ovan/under-operator)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


