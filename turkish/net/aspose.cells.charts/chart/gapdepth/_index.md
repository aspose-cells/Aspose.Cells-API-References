---
title: "Chart.GapDepth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3B bir grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır."
type: docs
url: /tr/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

3‑D grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır.

```csharp
public int GapDepth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // GapDepth özelliğini ayarla (3B grafiklerde veri serileri arasındaki mesafeyi kontrol eder)
            chart.GapDepth = 150; // Value between 0-500

            // Çalışma kitabını kaydedin
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


