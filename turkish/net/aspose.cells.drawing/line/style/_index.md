---
title: "Line.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Çizginin stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Çizgi stilini temsil eder.

```csharp
public LineType Style { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek bir grafik oluşturun
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // İlk seriyi ve onun ilk noktasını alın
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Çizgi özelliklerini ayarlayın
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Stilin ayarlandığını doğrulayın
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


