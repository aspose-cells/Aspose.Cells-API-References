---
title: "Chart.RotationAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3B grafik görünümünün döndürülmesini, çizim alanının z ekseni etrafındaki döndürülmesini derece cinsinden temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

3-B grafik görünümünün dönüşünü temsil eder (çizim alanının z ekseni etrafındaki dönüşü, derece cinsinden).

```csharp
public int RotationAngle { get; set; }
```

### Açıklamalar

Bu özelliğin değeri 0 ile 360 arasında olmalıdır, 3-D çubuk grafikler için ise değer 0 ile 44 arasında olmalıdır. Varsayılan değer 20'dir. Yalnızca 3-D grafiklerde uygulanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // Dönüş açısını 45 dereceye ayarla
            chart.RotationAngle = 45;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


