---
title: "MatrixEquationNode.BaseJc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MatrixEquationNode‑egenskap. Detta attribut anger justeringen av matrisen. Text utanför matrisen kan justeras med botten, toppen eller mitten av en matrisfunktion. Som standard antar matrisen centrerad justering"
type: docs
url: /sv/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Detta attribut specificerar justeringen av matrisen. Text utanför matrisen kan justeras med botten, toppen eller mitten av en matrisfunktion. Som standard antar matrisen centrerad justering.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyBaseJcDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationstycket och lägg till en matrisnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Ställ in matrisens egenskaper inklusive BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Lägg till 2x2‑matrisinnehåll (identitetsmatris)
            for (int row = 0; row < 2; row++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Spara arbetsboken
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Se även

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


