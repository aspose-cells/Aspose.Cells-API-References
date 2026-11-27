---
title: "AccentEquationNode.AccentCharacter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AccentEquationNode egenskap. Detta attribut specificerar typen av kombinerande diakritiskt tecken som är fäst vid basen för accentfunktionen. Standardaccenttecknet är U0302. Det rekommenderas starkt att använda attributet AccentType för att ställa in accenttecknet. Använd denna egenskapsinställning om du inte kan hitta det tecken du behöver i en känd typ."
type: docs
url: /sv/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Detta attribut specificerar typen av kombinerande diakritisk markör som är fäst vid basen av accentfunktionen. Standardaccenttecknet är U+0302. Det rekommenderas starkt att använda attributet AccentType för att ange accenttecken. Använd denna egenskapsinställning om du inte kan hitta tecknet du behöver i en känd typ.

```csharp
public string AccentCharacter { get; set; }
```

### Anmärkningar

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in, accepteras endast det första tecknet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden och lägg till en accentnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Ställ in accenttecknet (circumflex i detta fall)
            accentNode.AccentCharacter = "\u0302";

            // Lägg till bastext för accenten
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Spara arbetsboken
            workbook.Save("AccentEquationDemo.xlsx");

            // Verifiera den sparade filen genom att ladda tillbaka den
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Skriv ut accenttecknet för att demonstrera egenskapen
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Se även

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


