---
title: "Legend.Position"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Legend özelliği. Lejant konum tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Başlık konum tipini alır veya ayarlar.

```csharp
public LegendPositionType Position { get; set; }
```

### Açıklamalar

Varsayılan konum sağdır. Lejant grafik'in sol veya sağ tarafında ise, Legend.X özelliğini ayarlamak etkili olmaz. Lejant grafik'in üst veya alt tarafında ise, Legend.Y özelliğini ayarlamak etkili olmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Lejant konumunu ayarlayın
            chart.Legend.Position = LegendPositionType.Left;

            // Çalışma kitabını kaydedin
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


