---
title: "DisplayUnitLabel.AutoScaleFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DisplayUnitLabel özelliği. Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'tir."
type: docs
url: /tr/net/aspose.cells.charts/displayunitlabel/autoscalefont/
---
## DisplayUnitLabel.AutoScaleFont property

Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'dur.

```csharp
public override bool AutoScaleFont { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Görüntü birimi etiketini yapılandır
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Hundreds;
            Aspose.Cells.Charts.DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
            
            // AutoScaleFont özelliğini göster
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.Text = "100";

            workbook.Save("DisplayUnitLabelAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


