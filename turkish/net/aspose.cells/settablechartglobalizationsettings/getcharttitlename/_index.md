---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Grafik başlığının adını alır"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Grafik Başlığının adını alır.

```csharp
public override string GetChartTitleName()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Özel bir grafik başlığı adı ayarlayın
                settings.SetChartTitleName("Custom Chart Title");

                // GetChartTitleName kullanarak grafik başlığı adını alın
                string chartTitleName = settings.GetChartTitleName();

                // Sonucu göster
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Çalışma kitabını kaydedin
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


