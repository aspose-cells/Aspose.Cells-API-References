---
title: "Chart.FirstSliceAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart property. İlk piechart veya doughnutchart diliminin açısını, dikeyden saat yönünde derece cinsinden alır veya ayarlar. Yalnızca pie, 3D pie ve doughnut grafiklerinde 0 ile 360 arasında uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden alır veya ayarlar (dikeyden saat yönünde). Yalnızca pasta, 3‑D pasta ve halka grafiklerinde uygulanır, 0 ile 360 arasında.

```csharp
public int FirstSliceAngle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // İlk dilim açısını 45 dereceye ayarla
            chart.FirstSliceAngle = 45;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


