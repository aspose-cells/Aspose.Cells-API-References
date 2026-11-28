---
title: "Line.WeightPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Çizginin piksel birimindeki ağırlığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Çizginin ağırlığını piksel biriminde alır veya ayarlar.

```csharp
public double WeightPx { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Örnek veri ekleyin.
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Bir çizgi grafik ekle
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // WeightPx ile satır özelliklerini yapılandırın
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


