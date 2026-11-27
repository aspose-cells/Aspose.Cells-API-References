---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DelimiterEquationNode egenskap. Anger formen på avgränsare i avgränsningsobjektet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Specificerar formen på avgränsare i avgränsningsobjektet.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyDelimiterShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa avgränsningsnod med anpassad form
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // Lägg till innehåll inuti avgränsaren
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // Spara arbetsboken
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### Se även

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


