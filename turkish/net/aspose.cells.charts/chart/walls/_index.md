---
title: "Chart.Walls"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D grafiğin duvarlarını temsil eden bir Walls nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Bir `Walls` nesnesi döndürür; bu nesne 3‑D grafiğin duvarlarını temsil eder.

```csharp
public Walls Walls { get; }
```

### Açıklamalar

Bu özellik 3-D pasta grafiklerine uygulanmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Silindir sütun grafiği oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik temel ayarlarını yapılandır
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Duvar özelliklerini yapılandır
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Sonucu kaydet
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


