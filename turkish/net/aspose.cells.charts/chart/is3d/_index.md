---
title: "Chart.Is3D"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafiğin 3D grafik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Grafiğin 3D grafik olup olmadığını belirtir.

```csharp
public bool Is3D { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarla
            chart.SetChartDataRange("A1:B5", true);

            // Mevcut Is3D değerini göster
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Grafiğin 3D sürümünü oluştur
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // 3D grafiğin Is3D değerini göster
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


