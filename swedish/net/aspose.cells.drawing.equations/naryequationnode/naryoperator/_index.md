---
title: "NaryEquationNode.NaryOperator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode property. en n-är operator.t.ex . Det rekommenderas starkt att använda attributet NaryOperatorType för att ställa in n-är operator. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

en n-är operator.t.ex \"∑\". Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd denna egenskapsinställning om du inte kan hitta tecknet du behöver i en känd typ.

```csharp
public string NaryOperator { get; set; }
```

### Anmärkningar

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in, accepteras endast det första tecknet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en n-är operatornod
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Ställ in n-är operatoregenskaper
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Lägg till nedsänkt (valfritt)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Lägg till upphöjd (valfritt)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Lägg till basuttryck
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Spara arbetsboken
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Se även

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


