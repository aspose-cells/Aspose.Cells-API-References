---
title: "SlicerCache.CrossFilterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCache özelliği. Dilimleyicide veri olmayan öğelerin nasıl gösterileceğini belirtir"
type: docs
url: /tr/net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Veri olmayan dilimleyici öğelerinin nasıl gösterileceğini belirtir.

```csharp
[Obsolete("Use Slicer.ShowTypeOfItemsWithNoData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`ShowTypeOfItemsWithNoData`](../../slicer/showtypeofitemswithnodata/) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyCrossFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer ekle
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // CrossFilterType'ı ayarlayın ve gösterin
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
            Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);

            workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


