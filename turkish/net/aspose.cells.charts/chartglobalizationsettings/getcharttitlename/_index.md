---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartGlobalizationSettings yöntemi. Grafik başlığının adını alır"
type: docs
url: /tr/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

Grafik Başlığının adını alır.

```csharp
public virtual string GetChartTitleName()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek bir grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // ChartGlobalizationSettings örneği oluştur
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // GetChartTitleName yönteminin kullanımını gösterin
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


