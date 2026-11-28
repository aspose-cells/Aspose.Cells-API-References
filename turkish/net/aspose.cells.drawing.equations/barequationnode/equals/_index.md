---
title: "BarEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BarEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirleyin"
type: docs
url: /tr/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırma için iki BarEquationNode örneği oluşturun
            // Not: BarEquationNode'un gerçek oluşturulması API'nin fabrika yöntemlerine bağlı olacaktır
            // Demonstrasyon için, bunların doğru şekilde başlatılmış örnekler olduğunu varsayacağız
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // node1'i node2 ile karşılaştırın (eşit olmalı)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // node1'i node3 ile karşılaştırın (eşit olmamalı)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // node1'i null ile karşılaştırın
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // node1'i farklı bir nesne türüyle karşılaştırın
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // BarEquationNode almayı göstermek için yardımcı yöntem
        // Gerçek kullanımda, bunları oluşturmak için uygun API yöntemini kullanırsınız
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Bu sadece bir yer tutucudur - gerçek uygulama API'ye bağlı olacaktır
            // Örneğin, bir üst nesne veya fabrika yöntemi aracılığıyla oluşturulabilir
            return null; // Replace with actual creation code
        }
    }
}
```

### Ayrıca Bakınız

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


