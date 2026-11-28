---
title: "ChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartGlobalizationSettings yöntemi. Grafik için Diğer etiketlerinin adını alır"
type: docs
url: /tr/net/aspose.cells.charts/chartglobalizationsettings/getothername/
---
## ChartGlobalizationSettings.GetOtherName method

Grafik için "Other" etiketlerinin adını alır.

```csharp
public virtual string GetOtherName()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Küreselleştirme ayarlarını oluştur ve diğer adı al
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string otherName = globalizationSettings.GetOtherName();

            // Sonucu çıktı olarak ver
            Console.WriteLine("Other Name: " + otherName);

            // Çalışma kitabını kaydet
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


