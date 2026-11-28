---
title: "Axis.DisplayUnitLabel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Belirtilen grafikte bir eksende birim etiketini temsil eder. Birim etiketleri, milyonlar ya da milyarlar gibi büyük değerleri grafiklemek için faydalıdır."
type: docs
url: /tr/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Belirtilen grafikte bir eksende birim etiketini temsil eder. Birim etiketleri, milyonlar ya da milyarlar gibi büyük değerleri grafiklemek için faydalıdır.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:A4", true);
            
            // Görüntü birimini ve etiketi yapılandır
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Görüntü birimi etiket metnini çıktı al
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


