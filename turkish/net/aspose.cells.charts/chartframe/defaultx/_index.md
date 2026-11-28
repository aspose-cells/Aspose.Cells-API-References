---
title: "ChartFrame.DefaultX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Grafik alanının 1/4000 biriminde varsayılan konumun x'ini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Varsayılan konumun x'ini grafik alanının 1/4000 biriminde temsil eder.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.DefaultXRatioToChart özelliğini kullanın. DefaultX = (int)(DefaultXRatioToChart * 4000); Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // ChartFrame'den miras alan grafik başlığına erişin
            chart.Title.Text = "Sample Chart";
            
            // Grafik başlığının varsayılan X konumunu göster
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Varsayılan konumun grafiği nasıl etkilediğini gösterin
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // DefaultX yalnızca okunabilir olduğundan, oran özelliklerini kullanarak başlığın konumunu değiştirin
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


