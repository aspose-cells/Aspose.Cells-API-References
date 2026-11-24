---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MatrixEquationNode-Eigenschaft. Dieses Attribut gibt die Eigenschaft 'Hide Placeholders' einer Matrix an. Wenn diese Eigenschaft aktiviert ist, erscheinen Platzhalter nicht in der Matrix. Standardmäßig erscheinen Platzhalter, sodass die Stellen, an denen Text eingefügt werden kann, sichtbar gemacht werden"
type: docs
url: /de/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Dieses Attribut definiert die Eigenschaft Hide Placeholders für eine Matrix. Wenn diese Eigenschaft aktiviert ist, werden Platzhalter in der Matrix nicht angezeigt. Standardmäßig werden Platzhalter angezeigt, sodass die Stellen, an denen Text eingefügt werden kann, sichtbar sind.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ermitteln Sie den Math-Knoten und fügen Sie die Matrix hinzu
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Matrixeigenschaften festlegen
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Fügen Sie eine 2x2-Matrix mit Einsen auf der Diagonale hinzu
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Speichern und überprüfen
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


