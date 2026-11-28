---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable içinde PivotFieldSubtotalType tipinin metnini ayarlar"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

`[`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)` tipinin metnini PivotTable içinde ayarlar.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Bu [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| metin | String | Verilen tipin metni |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur (sadece gösterim amaçlı)
            Workbook workbook = new Workbook();

            // SettablePivotGlobalizationSettings örneği
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Sum alt toplamı için özel metin ayarlayın
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Değişikliği doğrulayın
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Average alt toplamı için özel metin ayarlayın
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Değişikliği doğrulayın
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Çalışma kitabını kaydet (bu demo'da pivot tablo değişikliği yok)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


