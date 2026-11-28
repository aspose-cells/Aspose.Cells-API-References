---
title: "ProtectedRange.GetAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange yöntemi. Başvurulan tüm alanları alır"
type: docs
url: /tr/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Tüm başvurulan alanları alır.

```csharp
public CellArea[] GetAreas()
```

### Dönüş Değeri

Başvurulan tüm alanları döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Korunan aralıklar koleksiyonunu al
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Bir korunan aralık ekle
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Korunan aralığın alanlarını al
            CellArea[] areas = protectedRange.GetAreas();
            
            // Alan sayısını çıktı olarak ver (bu basit aralık için 1 olmalı)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


