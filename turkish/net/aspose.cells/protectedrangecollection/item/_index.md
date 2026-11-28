---
title: "ProtectedRangeCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRangeCollection özelliği. Belirtilen indeksteki ProtectedRange öğesini alır"
type: docs
url: /tr/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Belirtilen indeksteki [`ProtectedRange`](../../protectedrange/) öğesini alır.

```csharp
public ProtectedRange this[int index] { get; }
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
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre indekslerini (startRow, startColumn, endRow, endColumn) kullanarak bir korumalı aralık ekleyin
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Item özelliğini (indeks 0) kullanarak korumalı aralığa erişin
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Koruma durumunu doğrulayın ve görüntüleyin
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


