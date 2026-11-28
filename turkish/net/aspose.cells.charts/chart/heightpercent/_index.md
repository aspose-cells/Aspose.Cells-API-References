---
title: "Chart.HeightPercent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D grafiğin yüksekliğini, grafik genişliğinin yüzde olarak 5 ile 500 arasında bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

3‑D grafiğin yüksekliğini, grafik genişliğinin yüzdesi olarak döndürür veya ayarlar (5 ile 500 yüzde arasında).

```csharp
public int HeightPercent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // HeightPercent özelliğini ayarla (3D grafiğin yüksekliğini grafik genişliğinin yüzde olarak kontrol eder)
            chart.HeightPercent = 150; // 150% of chart width

            // Çalışma kitabını kaydedin
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


