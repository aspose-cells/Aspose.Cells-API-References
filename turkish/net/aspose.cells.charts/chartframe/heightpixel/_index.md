---
title: "ChartFrame.HeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar.

```csharp
public virtual int HeightPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Grafik başlığına eriş (bu bir ChartFrame'dir)
            ChartFrame chartTitle = chart.Title;
            
            // Mevcut yüksekliği piksel olarak göster
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Başlık için yeni bir yükseklik ayarla
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Lejant'a eriş (başka bir ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Lejant yüksekliğini göster ve değiştir
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


