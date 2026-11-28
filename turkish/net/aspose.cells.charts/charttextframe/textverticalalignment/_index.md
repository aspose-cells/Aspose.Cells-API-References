---
title: "ChartTextFrame.TextVerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Metnin dikey hizalamasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

Metnin dikey hizalamasını alır veya ayarlar.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextVerticalAlignmentDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Başlığı ayarlayın ve dikey hizalamayı yapılandırın
            chart.Title.Text = "Sample Chart";
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Görüntü birimi etiketini yapılandırın
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
            chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");

            Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


