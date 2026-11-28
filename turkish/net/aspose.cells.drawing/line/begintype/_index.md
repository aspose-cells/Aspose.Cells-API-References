---
title: "Line.BeginType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Bir çizginin başlangıcı için ok ucu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Bir çizginin başlangıcı için ok başı belirtir.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Bir çizgi grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("A1:A3", true);

            // İlk seriyi alın ve çizgi özelliklerini yapılandırın
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Çalışma kitabını kaydedin
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


