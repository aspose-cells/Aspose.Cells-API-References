---
title: "UnionRange.Merge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Hücre aralığını tek bir hücreye birleştirir"
type: docs
url: /tr/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Bir hücre aralığını tek bir hücreye birleştirir.

```csharp
public void Merge()
```

### Açıklamalar

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1:B2 hücre aralığını oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Birleştirmeyi görselleştirmek için hücrelere bazı veriler koyun
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Aralıktan bir UnionRange oluşturun
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Merge yöntemini çağırın
                unionRange.Merge();
                
                // Birleştirilmiş hücreye değeri koyun
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Yorum satırını kaldırarak birleştirme kaldırmanın etkisini görün
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


