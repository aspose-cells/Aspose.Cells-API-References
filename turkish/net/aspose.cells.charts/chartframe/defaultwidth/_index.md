---
title: "ChartFrame.DefaultWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Grafik alanının 1/4000 birimi cinsinden varsayılan konumun genişliğini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Varsayılan konumun genişliğini grafik alanının 1/4000 birimi cinsinden temsil eder.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine ChartFrame.DefaultWidthRatioToChart özelliğini kullanın. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Grafik başlığına erişin (ChartFrame'den miras alır)
            Title title = chart.Title;
            
            // Grafik çerçevesinin varsayılan genişliğini gösterin (bu durumda başlık)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Not: DefaultWidth yalnızca okunabilir, bu yüzden ayarlanamaz
            // Varsayılan boyutları anlamak için yalnızca okuyabiliriz
            
            // Bu özelliğin grafiği nasıl etkilediğini gösterin
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


