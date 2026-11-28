---
title: "UnionRange.UnMerge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Bu aralığın birleştirilmiş hücrelerini ayırır"
type: docs
url: /tr/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Bu aralığın birleştirilmiş hücrelerini ayırır.

```csharp
public void UnMerge()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir aralık oluştur ve hücreleri birleştir
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Hücreleri birleştir ve bir değer koy
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // UnMerge yöntemini çağır
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Etkisini göstermek için ayrılmış hücrelere değerler koy
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


