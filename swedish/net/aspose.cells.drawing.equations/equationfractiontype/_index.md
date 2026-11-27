---
title: "Enum EquationFractionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationFractionType enum. Detta specificerar visningsstilen för bråkstrecket"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Detta specificerar visningsstilen för bråkstrecket.

```csharp
public enum EquationFractionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Bar | `0` | Detta specificerar att täljaren är ovanför och nämnaren nedanför, separerade av ett streck i mitten. |
| NoBar | `1` | Detta specificerar att täljaren är ovanför och nämnaren nedanför, men inte separerade av ett streck i mitten. |
| Linear | `2` | Detta specificerar att täljaren är till vänster och nämnaren till höger, separerade av ett '/' däremellan. |
| Skewed | `3` | Detta specificerar att täljaren är uppe till vänster och nämnaren nere till höger, separerade av ett "/". |

### Exempel

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
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta matematiknod och lägg till bråk
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Lägg till täljare
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Lägg till nämnare
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Spara och verifiera
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


