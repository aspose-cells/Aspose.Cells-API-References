---
title: "Chart.PageSetup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Bu grafikte sayfa ayarı açıklamasını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Bu grafikteki sayfa ayarı açıklamasını temsil eder.

```csharp
public PageSetup PageSetup { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekleyin ve grafik için bazı veriler ekleyin
            Worksheet dataSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            dataSheet.Name = "DataSheet";
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);

            // Bir grafik sayfası ekleyin
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Grafik sayfasına bir grafik ekleyin
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafiğin PageSetup'ına erişin
            PageSetup pageSetup = chart.PageSetup;

            // Sayfa ayarı özelliklerini ayarla
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Metin ve görüntü ile üst bilgiyi ayarlayın
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Alt bilgiyi ayarlayın
            pageSetup.SetFooter(0, "Page &P of &N");

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


