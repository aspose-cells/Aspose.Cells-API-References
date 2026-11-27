---
title: "ShapeCollection.AddEquation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till ett ekvationsobjekt i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Lägger till ett ekvationsobjekt i kalkylbladet.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Index för översta raden. |
| top | Int32 | Vertikal förskjutning för dess översta rad, i pixelenheter. |
| leftColumn | Int32 | Det vänstra kolumnindexet. |
| vänster | Int32 | Den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Höjden på ekvationen, i enhet pixel. |
| bredd | Int32 | Bredden på ekvationen, i enhet pixel. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fraction.FractionType = EquationFractionType.Skewed;

            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numText.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denText.Text = "B";

            workbook.Save("ShapeEquationDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


