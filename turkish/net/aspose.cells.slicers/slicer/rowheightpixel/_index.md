---
title: "Slicer.RowHeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer özelliği. Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar."
type: docs
url: /tr/net/aspose.cells.slicers/slicer/rowheightpixel/
---
## Slicer.RowHeightPixel property

Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar.

```csharp
public int RowHeightPixel { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyRowHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(40);

            // Özet tablo oluştur
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Dilimleyici ekle ve referansını al
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Dilimleyici özelliklerini ayarla
            slicer.RowHeightPixel = 30;
            slicer.Width = 150;

            workbook.Save("SlicerRowHeightDemo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


