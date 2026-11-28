---
title: "EquationNode.InsertAfter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode metodu. Belirtilen düğümü mevcut düğümün ardından ekler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Belirtilen düğümü geçerli düğümün sonrasına ekler.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresinde bir denklem şekli oluşturun
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // İlk metin düğümünü ekleyin
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Mevcut düğümün ardından yeni bir metin düğümü ekleyin
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Denklem yapısını gösterin
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Denklemi görsel inceleme için bir hücreye kaydedin
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


