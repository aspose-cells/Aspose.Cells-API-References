---
title: "DataLabels.ApplyFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels yöntemi. Veri etiketlerinin yazı tipini tüm alt düğümlere uygula"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Veri etiketlerinin yazı tipini tüm alt düğümlere uygula.

```csharp
public void ApplyFont()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Veri etiketlerini göster
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Veri etiketleri için yeni yazı tipi rengini ayarla
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Yazı tipi ayarlarını tüm veri etiketlerine uygula
            series.DataLabels.ApplyFont();
            
            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


