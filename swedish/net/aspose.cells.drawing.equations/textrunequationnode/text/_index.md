---
title: "TextRunEquationNode.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextRunEquationNode-egenskap. Ställ in innehållet i textnoden – vanligtvis ett nodobjekt per tecken"
type: docs
url: /sv/net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Ställ in innehållet i textnoden (Vanligtvis ett nodobjekt per tecken).

```csharp
public string Text { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Hämta rot-ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en bråkekvation
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Lägg till täljare med texten "X"
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Lägg till nämnare med texten "Y"
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Spara arbetsboken
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            // Verifiera den sparade filen genom att ladda tillbaka den
            Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Åtkomst till textegenskaperna för att demonstrera funktionaliteten
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

### Se även

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


