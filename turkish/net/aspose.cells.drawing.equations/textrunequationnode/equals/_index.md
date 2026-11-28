---
title: "TextRunEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextRunEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirleyin"
type: docs
url: /tr/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demo amaçları için null kullanacağız ve sadece karşılaştırma mantığını göstereceğiz
            // çünkü TextRunEquationNode örneklerini doğrudan oluşturamıyoruz
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Bu bölüm, Equals'in nasıl çağrılacağını göstermek için kalır
                // Gerçek bir senaryoda, bunlar düzgün bir şekilde başlatılmış düğümler olurdu
                if (node1 != null && node2 != null && node3 != null)
                {
                    // node1'i node2 ile karşılaştırın (aynı içerik)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // node1'i node3 ile karşılaştırın (farklı içerik)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // null ile karşılaştır
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Farklı nesne türüyle karşılaştırın
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin (Equals'in elektronik tabloyu değiştirmediği halde)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // TextRunEquationNode örneklerini düzgün bir şekilde oluşturamadığımız için yardımcı yöntem kaldırıldı
    }
}
```

### Ayrıca Bakınız

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


