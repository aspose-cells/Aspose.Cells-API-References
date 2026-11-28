---
title: "TickLabels.RotationAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. Metnin saat yönünde döndürme açısını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Metin dönüş açısını saat yönünde temsil eder.

```csharp
public int RotationAngle { get; set; }
```

### Açıklamalar

0: Döndürülmedi.255: Yukarıdan Aşağıya.-90: Aşağı yön.90: Yukarı yön.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Kategori ekseni tick etiketlerini 45 derece döndür
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


