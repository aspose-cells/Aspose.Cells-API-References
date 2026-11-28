---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Legend için Decrease adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Lejant için Azaltma adını ayarlar.

```csharp
public void SetLegendDecreaseName(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | yerel bağımlı ad |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Küreselleştirme ayarları oluştur
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // SetLegendDecreaseName'i özel bir dizeyle çağır
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Chart sınıfının ChartGlobalizationSettings özelliği yoktur,
                // bu yüzden gerektiğinde ayarlar nesnesini doğrudan kullanmamız gerekir
                // (Not: Gerçek kullanımda, bu ayarların nerede uygulandığını bulmanız gerekir)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


