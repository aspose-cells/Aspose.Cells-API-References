---
title: "Chart.RightAngleAxes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafik eksenleri dik açıdaysa doğru. Yalnızca 3D grafikler için geçerlidir, Column3D ve 3D Pie Charts hariç."
type: docs
url: /tr/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

Grafik eksenleri dik açıdaysa True. Yalnızca 3-B grafikler için geçerlidir (Column3D ve 3-B Pasta Grafikleri hariç).

```csharp
public bool RightAngleAxes { get; set; }
```

### Açıklamalar

Bu özellik doğru ise, Perspective özelliği göz ardı edilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // RightAngleAxes özelliğini göster
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Çalışma kitabını kaydedin
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


