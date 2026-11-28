---
title: "SlicerCacheItem.Selected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCacheItem özelliği. SlicerCacheItem'ın seçili olup olmadığını belirtir"
type: docs
url: /tr/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

[`SlicerCacheItem`](../) öğesinin seçili olup olmadığını belirtir.

```csharp
public bool Selected { get; set; }
```

### Açıklamalar

Öğe seçmek istiyorsanız, lütfen bunun yerine [`SelectItems`](../../slicer/selectitems/) yöntemini kullanın. Çünkü bu yenileme işlemi, seçim her değiştiğinde tam veri yeniden yüklemesi nedeniyle düşük performansa neden olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Slicer ekle
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Slicer önbellek öğelerine eriş
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // İlk öğeyi seç, diğerlerinin seçimini kaldır
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


