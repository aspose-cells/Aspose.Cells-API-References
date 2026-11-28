---
title: "Sınıf SettableChartGlobalizationSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SettableChartGlobalizationSettings sınıfı. Kullanıcının önceden tanımlı metinleri ayarlamasını/değiştirmesini destekleyen PivotGlobalizationSettings uygulaması"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan PivotGlobalizationSettings uygulaması.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Eksen için Başlık adını alır. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Eksen biriminin adını alır. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Grafik Başlığının adını alır. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Lejant için Azaltma adını alır. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Lejant için Artırma adını alır. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Lejant için Toplam adını alır. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Grafik için "Other" etiketlerinin adını alır. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Grafikteki Serinin adını alır. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Eksen için Başlık adını ayarlar. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Eksen biriminin adını ayarlar. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Grafik Başlığının adını ayarlar. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Lejant için Azaltma adını ayarlar. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Lejant için Artırma adını ayarlar. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Lejant için Toplam adını ayarlar. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Grafik için "Other" etiketlerinin adını ayarlar. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Grafikteki Serinin adını ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // SettableChartGlobalizationSettings örneği oluştur
                var settings = new SettableChartGlobalizationSettings();

                // Özel küreselleştirme ayarlarını ayarla
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Özel bir GlobalizationSettings uygulaması oluştur
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Ayarları göstermek için basit bir grafik oluştur
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // Gerekli GlobalizationSettings yöntemlerini burada uygula
            // SettableChartGlobalizationSettings örneğine delege eden
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


