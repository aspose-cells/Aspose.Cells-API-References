---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MatrixEquationNode‑egenskap. Detta attribut anger egenskapen Hide Placeholders på en matris. När detta attribut är aktiverat visas inte platshållare i matrisen. Standardplatshållare visas så att de platser där text kan infogas blir synliga"
type: docs
url: /sv/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Detta attribut specificerar egenskapen Hide Placeholders på en matris. När denna egenskap är aktiverad visas inte platshållare i matrisen. Som standard visas platshållare så att de platser där text kan infogas blir synliga.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Exempel

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
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta matematiknod och lägg till matris
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Ställ in matrisens egenskaper
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Lägg till en 2x2-matris med diagonala 1:or
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

            // Spara och verifiera
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


