---
title: "SlicerCache.List"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCache özelliği. Belirtilen slicer önbelleğiyle ilişkili diliminin NonOLAP veri kaynağına dayanıp dayanmadığını gösterir."
type: docs
url: /tr/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Belirtilen slicer önbelleğiyle ilişkili slicer'ın Non-OLAP veri kaynağına dayanıp dayanmadığını belirtir.

```csharp
public bool List { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyListDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Doğru aşırı yükleme ile tablo oluştur
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Slicer ekle
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Slicer önbelleğine eriş
            SlicerCache cache = slicer.SlicerCache;

            // List özelliğinin kullanımını göster
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### Ayrıca Bakınız

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


