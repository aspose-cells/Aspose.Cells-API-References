---
title: "BoxEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BoxEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğümle eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırma için iki BoxEquationNode nesnesi oluşturun
            // BoxEquationNode parametresiz bir yapıcıya sahip olmadığından,
            // farklı bir şekilde oluşturmamız gerekecek. Bir yerden alabileceğimizi varsayarak,
            // veya bazı varsayılan parametrelerle oluşturabilirsiniz.
            // Demo amaçlı, sadece onları bildirecek ve null atayacağız (gerçek kodda ise uygun başlatma gerekir)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Equals yöntemini belirli parametre tipleriyle (Object) çağırın
                    bool areEqual = node1.Equals(objToCompare);

                    // Sonucu göster
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Sonucu çalışma sayfasına ekleyin
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Sonucu kaydet
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


