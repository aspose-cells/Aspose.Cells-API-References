---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection yöntemi. Biçimlendirme koşulunu indeksle kaldırır"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Biçimlendirme koşulunu dizine göre kaldırır.

```csharp
public void RemoveCondition(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Kaldırılacak biçimlendirme koşulunun indeksi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biçim koşulları koleksiyonunu al
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Bazı örnek koşullar ekle
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // İlk sayıyı göster
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // İlk koşulu kaldır
                formatConditions.RemoveCondition(index1);
                
                // Güncellenmiş sayıyı göster
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


