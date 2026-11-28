---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MatrixEquationNode özelliği. Bu öznitelik bir matris üzerindeki Gizli Yer Tutucular özelliğini belirtir. Bu özellik etkin olduğunda yer tutucular matris içinde görünmez. Varsayılan yer tutucular görünür, böylece metnin eklenebileceği konumlar görülebilir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Bu öznitelik, bir matris üzerindeki Yer Tutucuları Gizle özelliğini belirtir. Bu özellik açık olduğunda, yer tutucular matris içinde görünmez. Varsayılan olarak, yer tutucular görünür, böylece metnin eklenebileceği konumlar görülebilir.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Örnekler

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
            
            // Denklem şekli ekle
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Matematik düğümünü alın ve matrisi ekleyin
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Matris özelliklerini ayarla
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // köşegeninde 1'ler olan 2x2 matris ekleyin
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

            // Kaydet ve doğrula
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


