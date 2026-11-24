---
title: "MatrixEquationNode.BaseJc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MatrixEquationNode-Eigenschaft. Dieses Attribut gibt die Ausrichtung der Matrix an. Text außerhalb der Matrix kann mit dem unteren, oberen oder mittleren Teil einer Matrixfunktion ausgerichtet werden. Standardmäßig nimmt die Matrix die mittlere Ausrichtung an"
type: docs
url: /de/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Dieses Attribut gibt die Ausrichtung der Matrix an. Text außerhalb der Matrix kann am unteren, oberen oder mittleren Teil einer Matrixfunktion ausgerichtet werden. Standardmäßig nimmt die Matrix eine zentrierte Ausrichtung an.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie dem ersten Arbeitsblatt eine Gleichungsform hinzu.
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Holen Sie den Gleichungsabsatz und fügen Sie einen Matrixknoten hinzu
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Setzen Sie Matrixeigenschaften einschließlich BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Fügen Sie 2x2-Matrixinhalt (Einheitsmatrix) hinzu
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

            // Speichere die Arbeitsmappe
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Siehe auch

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


