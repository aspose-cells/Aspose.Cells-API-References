---
title: "EquationNodeParagraph.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNodeParagraph yöntemi. Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Belirtilen düğüm |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırma için iki EquationNodeParagraph örneği oluşturun
            // CreateNode metodunu kullanarak düğümleri doğru şekilde örnekleyin
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Farklı hizalama türleri ayarlayarak onları eşit olmayan hâle getirin
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Equals metodunu paragraph2 parametresiyle çağırın
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // paragraph1 ile aynı hizalamaya sahip başka bir paragraf oluşturun
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Paragraph3 ile tekrar Equals çağırın
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // Ayrıca null ile karşılaştırmayı gösterin
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin (ancak çalışma sayfasına görünür bir değişiklik yapılmadı)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


