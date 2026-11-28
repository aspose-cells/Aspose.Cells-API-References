---
title: "EquationNode.InsertBefore"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Belirtilen düğümü mevcut düğümün önüne ekler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Belirtilen düğümü geçerli düğümün öncesine ekler.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | EquationNodeType | Denklem Düğümlerinin Türleri |

### Dönüş Değeri

Belirtilen tür mevcutsa, karşılık gelen düğüm döndürülür; tür mevcut değilse, bilinmeyen türde bir düğüm döndürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresinde matematiksel bir denklem oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Denkleme başlangıç metin düğümünü ekle
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Mevcut olanın önüne yeni bir metin düğümü ekle
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Denklemi LaTeX formatında göster
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


