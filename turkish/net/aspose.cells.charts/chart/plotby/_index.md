---
title: "Chart.PlotBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Satır mı yoksa sütun mu çizileceğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Satır veya sütun bazında çizim yapılıp yapılmayacağını alır ve ayarlar.

```csharp
public PlotDataByType PlotBy { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.SetChartDataRange("A1:C4", true);

            // PlotBy özelliğini göster
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Farklı plot ayarıyla yeni bir grafik oluştur
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


