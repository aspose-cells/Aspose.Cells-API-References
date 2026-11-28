---
title: "ChartFrame.YPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar.

```csharp
public virtual int YPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
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

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığına erişin (ChartFrame'den miras alır)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // Mevcut YPixel değerini göster
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // Grafik başlığının YPixel konumunu değiştir
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


