---
title: "SettablePivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable'da boş etiketin metnini alır"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

PivotTable'daki "(blank)" etiketinin metnini alır.

```csharp
public override string GetTextOfEmptyData()
```

### Dönüş Değeri

Boş verinin metni

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // SettablePivotGlobalizationSettings bir örnek oluştur
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Boş veri için varsayılan metni al
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // Boş veri için özel metin ayarla
                settings.SetTextOfEmptyData("No Data Available");

                // Boş veri için güncellenmiş metni al
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // Ayarları çalışma kitabına uygula
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Çalışma kitabını kaydedin
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


