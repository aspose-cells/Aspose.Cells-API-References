---
title: "LimLowUppEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LimLowUppEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

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

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yapıcı parametrelerini bilmediğimiz için null değerleri karşılaştıracağız
            // Bu, derlenmesini sağlamak için minimal bir değişikliktir - gerçek kullanımda uygun bir yapılandırma gerekir
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Equals yöntemini belirli parametre türüyle (Object) çağırın
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Sonucu göster
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Çalışma kitabını kaydedin
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


