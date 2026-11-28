---
title: "Chart.AutoScaling"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Microsoft Excel bir 3D grafiği, eşdeğer 2D grafiğe boyut olarak daha yakın olacak şekilde ölçeklendiriyorsa doğru. RightAngleAxes özelliği de doğru olmalıdır"
type: docs
url: /tr/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

Microsoft Excel bir 3D grafiği, eşdeğer 2D grafiğe boyut olarak daha yakın olacak şekilde ölçeklendiriyorsa True. RightAngleAxes özelliği True olmalıdır.

```csharp
public bool AutoScaling { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // AutoScaling özelliğini göster
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


