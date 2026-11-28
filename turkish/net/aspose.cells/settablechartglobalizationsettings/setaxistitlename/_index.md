---
title: "SettableChartGlobalizationSettings.SetAxisTitleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Eksen için Başlık adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Eksen için Başlık adını ayarlar.

```csharp
public void SetAxisTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için minimum veri ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // SettableChartGlobalizationSettings örneği oluştur
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Özel bir eksen başlığı adı ayarla
                settings.SetAxisTitleName("Custom Axis Title");

                // Eksen başlık adını alarak ayarı doğrulayın
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Çalışma kitabını kaydedin
                workbook.Save("SetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


