---
title: "Chart.Elevation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D grafik görünümünün yüksekliğini derece cinsinden temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

3‑D grafik görünümünün yüksekliğini derece cinsinden temsil eder.

```csharp
public int Elevation { get; set; }
```

### Açıklamalar

Grafik yüksekliği, grafiği gördüğünüz yüksekliği dereceler cinsinden ifade eder. Çoğu grafik türü için varsayılan değer 15'tir. Bu özelliğin değeri -90 ile 90 arasında olmalıdır, 3-D çubuk grafikleri için ise 0 ile 44 arasında olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Yükseklik özelliğini ayarla (derece cinsinden açı)
            chart.Elevation = 30;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


