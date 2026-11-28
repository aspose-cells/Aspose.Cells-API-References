---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable'daki Grand Total etiketi metnini ayarlar"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

PivotTable'daki "Grand Total" etiketinin metnini ayarlar.

```csharp
public void SetTextOfGrandTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun (yalnızca bağlam için)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // SettablePivotGlobalizationSettings örneği
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // "Grand Total" etiketi için özel bir metin ayarlayın
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Değişikliği doğrulamak için güncellenen etiket metnini alın
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Kodun hatasız çalıştığını göstermek için çalışma kitabını kaydedin
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


