---
title: "ShapeCollection.AddEquation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un oggetto equazione al foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Aggiunge un oggetto equazione al foglio di lavoro.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | L'indice della riga superiore. |
| alto | Int32 | Lo scostamento verticale della sua riga superiore, in unità di pixel. |
| leftColumn | Int32 | L'indice della colonna sinistra. |
| sinistra | Int32 | Lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | L'altezza dell'equazione, in unità di pixel. |
| larghezza | Int32 | La larghezza dell'equazione, in unità di pixel. |

### Esempi

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

### Vedi anche

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


