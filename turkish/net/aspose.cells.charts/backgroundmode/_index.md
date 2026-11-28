---
title: "Enum BackgroundMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.BackgroundMode enum. Arka planın görüntüleme modunu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Arka planın görüntüleme modunu temsil eder.

```csharp
public enum BackgroundMode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik |
| Opaque | `1` | Opak |
| Transparent | `2` | Şeffaf |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasının referansını alın.
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleyin
            chart.NSeries.Add("A1:B3", true);
            
            // Grafik alanına eriş
            ChartArea chartArea = chart.ChartArea;

            // Grafik alanının ön plan rengini ayarla
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Grafik alanının arka plan modunu ayarla
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Grafik alanının gölgesini ayarla
            chartArea.Shadow = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


