---
title: "Enum EquationDelimiterShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType enum. Detta specificerar formen på avgränsare i avgränsningsobjektet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Detta specificerar formen på avgränsare i avgränsarobjektet.

```csharp
public enum EquationDelimiterShapeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Centered | `0` | Avdelaren är centrerad runt hela höjden av dess innehåll. |
| Match | `1` | Avdelaren har ändrats för att exakt matcha höjden på deras innehåll. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Hämta ekvationsnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa avgränsningsnod med Match-formtyp
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Lägg till innehåll inuti avgränsaren
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Spara arbetsboken
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


