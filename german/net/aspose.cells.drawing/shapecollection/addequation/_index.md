---
title: "ShapeCollection.AddEquation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Der Index der obersten Zeile. |
| oben | Int32 | Der vertikale Versatz seiner oberen Zeile, in Pixeln. |
| leftColumn | Int32 | Der Index der linken Spalte. |
| links | Int32 | Der horizontale Versatz von seiner linken Spalte, in Pixeln. |
| Höhe | Int32 | Die Höhe der Gleichung, in Pixeln. |
| Breite | Int32 | Die Breite der Gleichung, in Pixeln. |

### Beispiele

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

### Siehe auch

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


