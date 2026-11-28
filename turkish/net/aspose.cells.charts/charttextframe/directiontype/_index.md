---
title: "ChartTextFrame.DirectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Metnin yönünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Metnin yönünü alır ve ayarlar.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // Bir çalışma sayfası eklemek, dizinini döndürür, ardından çalışma sayfasını dizinle alırız
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Başlığı erişin ve yapılandırın
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // DirectionType özelliğini gösterin
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


