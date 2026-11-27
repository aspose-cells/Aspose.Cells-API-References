---
title: "DelimiterEquationNode.EndChar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DelimiterEquationNode egenskap. Avgränsare sluttecken"
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

Avgränsningens sluttecken.

```csharp
public string EndChar { get; set; }
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
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en avgränsningsnod med anpassat sluttecken
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // Lägg till innehåll inuti avgränsaren
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // Spara och verifiera
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Verifiera den sparade filen
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### Se även

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


