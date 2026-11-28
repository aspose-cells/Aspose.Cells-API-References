---
title: "Walls.CenterY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Walls özelliği. Chart.Calculate yöntemini çağırdıktan sonra, grafiğin yüksekliğinin 1/4000 birimi cinsinden Wall merkezinin sol-alt köşesinin y koordinatını alır."
type: docs
url: /tr/net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin y koordinatını, grafiğin yüksekliğinin 1/4000 birimi cinsinden alır.

```csharp
public int CenterY { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYDemo
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

            // 3D bir grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özellikleri güncelle
            chart.Calculate();

            // Walls öğesine erişin ve CenterY özelliğini gösterin
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterY position: " + walls.CenterY);

            // Çalışma kitabını kaydedin
            workbook.Save("WallsCenterYDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


