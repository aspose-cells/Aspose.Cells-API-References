---
title: "Series.SizeRepresents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Balon grafiğinde balon boyutunun neyi temsil ettiğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Baloncuk grafiğinde baloncuk boyutunun neyi temsil ettiğini alır veya ayarlar.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Açıklamalar

BubbleSizeRepresents.SizeIsArea, [`BubbleSizes`](../bubblesizes/) değerinin balonun alanı olduğunu ifade eder. BubbleSizeRepresents.SizeIsWidth, [`BubbleSizes`](../bubblesizes/) değerinin balonun genişliği olduğunu ifade eder.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Balon grafiği için örnek veri ekle
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Bir balon grafiği ekle
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Seri verilerini ayarla
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // SizeRepresents özelliğini ayarla
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


