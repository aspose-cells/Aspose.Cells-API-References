---
title: "DelimiterEquationNode.BeginChar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DelimiterEquationNode egenskap. Avgränsare starttecken"
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

Avgränsningens starttecken.

```csharp
public string BeginChar { get; set; }
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
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvation i det första kalkylbladet
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Hämta ekvationens rotnod
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Lägg till en avgränsningsnod med anpassade start‑/sluttecken
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // Lägg till innehåll inuti avgränsaren
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // Spara arbetsboken
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### Se även

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


