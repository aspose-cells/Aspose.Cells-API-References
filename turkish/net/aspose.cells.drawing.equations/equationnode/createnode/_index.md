---
title: "EquationNode.CreateNode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Belirtilen türde bir düğüm oluştur"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Belirtilen tipte bir düğüm oluştur.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | EquationNodeType | Denklem Düğümlerinin Türleri |
| çalışma kitabı | Çalışma Kitabı | Denkleme ilişkin çalışma kitabı nesnesi |
| üst | EquationNode | Bu düğümün bulunduğu üst düğüm |

### Dönüş Değeri

Belirtilen tür mevcutsa, karşılık gelen düğüm döndürülür; tür mevcut değilse, bilinmeyen türde bir düğüm döndürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir denklem şekli oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Bir üst düğüm (kesir) oluştur
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Pay ve payda düğümlerini oluştur
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Oluşturulan kesiri ana denkleme ekle
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Denklemi bir hücrede göster
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


