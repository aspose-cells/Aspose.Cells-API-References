---
title: "Chart.ShowLegend"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafiğin açıklama kutusunun gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Grafik açıklamasının gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer true.

```csharp
public bool ShowLegend { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Açıklama kutusunu varsayılan olarak göster (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Açıklama kutusunu gizle
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


