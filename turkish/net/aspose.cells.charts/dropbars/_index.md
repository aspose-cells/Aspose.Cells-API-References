---
title: "Class DropBars"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.DropBars sınıfı. Bir grafikteki yukarı ve aşağı çubukları temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/dropbars/
---
## DropBars class

Grafikteki yukarı ve aşağı çubukları temsil eder.

```csharp
public class DropBars
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | `[Area`](./area/) öğesini alır. |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Sınır `[Line`](../../aspose.cells.drawing/line/) öğesini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleyin
            chart.NSeries.Add("A1:B3", true);

            // Yukarı ve aşağı çubukları etkinleştir
            chart.NSeries[0].HasUpDownBars = true;

            // DropBars nesnesine eriş
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Yukarı çubukların görünümünü özelleştir
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Aşağı çubukların görünümünü özelleştir
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Çalışma kitabını kaydedin
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


