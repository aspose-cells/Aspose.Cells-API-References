---
title: "Slicer.StyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer özelliği. Yerleşik dilimleyici stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1'dir"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/styletype/
---
## Slicer.StyleType property

Yerleşik dilimleyici stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1.

```csharp
public SlicerStyleType StyleType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyStyleTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Slicer ekle
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // StyleType dahil olmak üzere dilimleyici özelliklerini ayarlayın
            slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
            slicer.Caption = "Fruit Selection";
            slicer.NumberOfColumns = 2;
            slicer.Width = 200;
            slicer.Height = 100;

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


