---
title: "UnknowEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnknowEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirleyin"
type: docs
url: /tr/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırma için iki bilinmeyen denklem düğümü oluşturun
            // UnknowEquationNode parametresiz bir yapıcıya sahip olmadığı için,
            // onları farklı bir şekilde oluşturmamız gerekecek. Demo amaçlı, şunu kullanacağız
            // eğer mevcutsa gerçek yapıcıyı, ya da başka yollarla oluşturmayı.
            // Yapıcı parametrelerini bilmediğimiz için, bu bir yer tutucu düzeltmedir.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Equals yöntemini belirli parametre türüyle (Object) çağırın
                bool areEqual = node1.Equals(objToCompare);

                // Sonucu göster
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Sonucu çalışma sayfasına ekleyin
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // UnknowEquationNode örnekleri oluşturmak için yardımcı yöntem
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // Gerçek bir uygulamada, bu uygun yapıcıyı kullanırdı
            // Yapıcı parametrelerini bilmediğimiz için, null döndüreceğiz
            // ve demo içinde null durumunu ele alacağız (bu sadece bir yer tutucudur)
            return null;
        }
    }
}
```

### Ayrıca Bakınız

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


