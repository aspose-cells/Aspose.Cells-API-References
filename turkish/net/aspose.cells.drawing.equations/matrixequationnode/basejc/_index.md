---
title: "MatrixEquationNode.BaseJc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MatrixEquationNode özelliği. Bu öznitelik matrisin hizalamasını belirtir. Matrisin dışındaki metin, matris fonksiyonunun alt, üst veya ortasıyla hizalanabilir. Varsayılan olarak matris orta hizalamayı varsayar."
type: docs
url: /tr/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Bu öznitelik, matrisin hizalamasını belirtir. Matrisin dışındaki metin, matris işlevinin altına, üstüne veya ortasına hizalanabilir. Varsayılan olarak, matris ortalanmış hizalama varsayar.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem şekli ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklem paragrafını al ve bir matris düğümü ekle
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // BaseJc dahil olmak üzere matris özelliklerini ayarlayın
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // 2x2 matris içeriği ekleyin (birim matris)
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

            // Çalışma kitabını kaydedin
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


