---
title: "SettablePivotGlobalizationSettings.SetTextOfTotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable'daki Toplam etiketi metnini ayarlar"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

PivotTable'daki "Total" etiketinin metnini ayarlar.

```csharp
public void SetTextOfTotal(string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | özel metin |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı örnek veriler ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // SettablePivotGlobalizationSettings bir örnek oluştur
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // "Total" varsayılan metnini alın
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // "Total" için özel bir metin ayarlayın
                settings.SetTextOfTotal("Custom Total Label");

                // Değişikliği doğrulayın
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // Çalışma kitabını kaydedin
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


