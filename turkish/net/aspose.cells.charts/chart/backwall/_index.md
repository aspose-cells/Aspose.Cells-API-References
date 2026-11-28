---
title: "Chart.BackWall"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. 3D grafiğin arka duvarını temsil eden bir Walls nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Bir [`Walls`](../walls/) nesnesi döndürür; bu nesne 3‑D grafiğin arka duvarını temsil eder.

```csharp
public Walls BackWall { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // 3D sütun grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Bunun bir 3D grafik olduğundan emin olun
            if (chart.Is3D)
            {
                // BackWall nesnesini alın
                Walls backWall = chart.BackWall;

                // BackWall'un bazı özelliklerini göster
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // BackWall'u biçimlendir
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Kenarlık özelliklerini ayarla
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


