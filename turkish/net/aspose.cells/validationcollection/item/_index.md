---
title: "ValidationCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ValidationCollection özelliği. Belirtilen indeksteki Validation öğesini alır"
type: docs
url: /tr/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Belirtilen indeksteki [`Validation`](../../validation/) öğesini alır.

```csharp
public Validation this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hücrelere veri doğrulaması ekle
            ValidationCollection validations = sheet.Validations;
            
            // İlk doğrulama alanı
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // İkinci doğrulama alanı
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Item özelliğini kullanarak doğrulamaya eriş
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Alanları doğrula
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


