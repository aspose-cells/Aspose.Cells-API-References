---
title: "FormatConditionCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection özelliği. Biçimlendirme koşulunu dizine göre alır"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Biçimlendirme koşulunu dizine göre alır.

```csharp
public FormatCondition this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | dönülecek biçimlendirme koşulunun dizini. |

### Dönüş Değeri

biçimlendirme koşulu

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bir biçim koşulu koleksiyonu ekle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Bir biçim koşulu ekle
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Item özelliğini kullanarak ilk biçim koşuluna erişin
            FormatCondition condition = fcc[0];
            
            // Formülleri göster
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Item özelliğini kullanarak formülleri değiştir
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Değiştirilmiş formülleri göster
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


