---
title: "SettableChartGlobalizationSettings.SetLegendIncreaseName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Legend için artış adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Lejant için Artırma adını ayarlar.

```csharp
public void SetLegendIncreaseName(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | yerel bağımlı ad |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için minimum veri ekle
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // SettableChartGlobalizationSettings örneği oluştur
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Özel bir lejant artış adı ayarlayın
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Değeri alarak ayarı doğrulayın
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Çalışma kitabını kaydedin
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


