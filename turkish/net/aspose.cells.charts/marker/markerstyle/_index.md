---
title: "Marker.MarkerStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Marker özelliği. İşaretçi stilini temsil eder. Çizgi grafiği, dağılım grafiği veya radar grafiği için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

İşaretçi stilini temsil eder. Çizgi grafiği, dağılım grafıği veya radar grafiği için geçerlidir.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // İlk seri için işaretçi stilini ayarla
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Çalışma kitabını kaydedin
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


