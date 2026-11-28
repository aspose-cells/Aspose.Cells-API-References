---
title: "Range.UnMerge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu aralıktaki birleştirilmiş hücrelerin birleştirmesini kaldırır"
type: docs
url: /tr/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Bu aralığın birleştirilmiş hücrelerini ayırır.

```csharp
public void UnMerge()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2'den D4'e kadar hücreleri birleştir
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // B2 hücresinin birleştirilmiş olup olmadığını birleştirmeyi kaldırmadan önce kontrol edin
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Aralığın birleştirmesini kaldır
            range.UnMerge();
            
            // B2 hücresinin birleştirilmiş olup olmadığını birleştirme kaldırıldıktan sonra kontrol edin
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


