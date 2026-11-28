---
title: "SlicerCacheItem.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCacheItem özelliği. Slicer öğesi için etiket metnini döndürür"
type: docs
url: /tr/net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

Slicer öğesi için etiket metnini döndürür.

```csharp
public string Value { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertyValueDemo
    {
        public static void Run()
        {
            // Örnek veriyle bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Özet tablo için örnek veri oluştur
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["A2"].PutValue("Alex");
            ws.Cells["A3"].PutValue("Sam");
            ws.Cells["A4"].PutValue("Alex");
            ws.Cells["A5"].PutValue("John");
            
            // Özet tablo oluştur
            int index = ws.PivotTables.Add("A1:A5", "E1", "PivotTable1");
            PivotTable pt = ws.PivotTables[index];
            pt.AddFieldToArea(PivotFieldType.Row, "Name");
            
            // Slicer ekle
            int slicerIndex = ws.Slicers.Add(pt, "Name", "Slicer1");
            Slicer slicer = ws.Slicers[slicerIndex];
            
            // Value özelliğinin kullanımını gösterin
            Console.WriteLine("All items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            // Yalnızca "Alex"'i seç
            Console.WriteLine("\nSelecting only Alex:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = (item.Value == "Alex");
            }
            slicer.Refresh();
            
            // Seçili öğeleri göster
            Console.WriteLine("\nSelected items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                if (item.Selected)
                {
                    Console.WriteLine(item.Value);
                }
            }
            
            // Tüm öğeleri seç
            Console.WriteLine("\nSelecting all items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = true;
            }
            slicer.Refresh();
        }
    }
}
```

### Ayrıca Bakınız

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


