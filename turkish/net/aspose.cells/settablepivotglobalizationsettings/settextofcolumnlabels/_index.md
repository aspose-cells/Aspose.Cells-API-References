---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable içinde Column Labels etiketinin metnini alır"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

PivotTable'daki "Column Labels" etiketinin metnini alır.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Sütun etiketlerinin metni |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur (sadece bağlam için)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // SettablePivotGlobalizationSettings bir örnek oluştur
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // \"Column Labels\" etiketi için özel metin ayarlayın
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Değişikliği doğrulamak için mevcut metni al
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Çalışma kitabını kaydet (bu demo için pivot tablo gerekmez)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


