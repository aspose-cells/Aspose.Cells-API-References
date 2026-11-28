---
title: "DisplayUnitLabel.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DisplayUnitLabel özelliği. Görüntü birimi etiketinin metnini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Görüntü birimi etiketinin metnini alır veya ayarlar.

```csharp
public override string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:A4", true);
            
            // Görüntü birimi etiketini yapılandır
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Görüntü birimi etiketinin metnine erişin ve değiştirin
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Metni değiştir
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Çalışma kitabını kaydedin
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


