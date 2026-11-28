---
title: "Chart.DepthPercent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D bir grafiğin derinliğini, grafik genişliğinin yüzde olarak 20 ile 2000 arasında bir yüzdesi olarak temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

3‑D bir grafiğin derinliğini, grafik genişliğinin yüzdesi olarak temsil eder (20 ile 2000 yüzde arasında).

```csharp
public int DepthPercent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
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
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // DepthPercent özelliğini ayarla (3D grafiğin derinliğini grafik genişliğinin yüzde olarak kontrol eder)
            chart.DepthPercent = 150; // 150% depth

            // Çalışma kitabını kaydedin
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


