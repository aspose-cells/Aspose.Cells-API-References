---
title: "CellWatch.CellName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellWatch özelliği. Hücrenin adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Hücrenin adını alır ve ayarlar.

```csharp
public string CellName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı hücre izlemeleri ekle
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Tüm izlemelerin hücre adlarını göster
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Yeni bir izleme ekle ve adını göster
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


