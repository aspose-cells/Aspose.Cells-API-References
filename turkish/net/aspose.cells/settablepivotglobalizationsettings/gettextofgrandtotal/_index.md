---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable'daki Grand Total etiketi metnini alır"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

PivotTable'daki "Grand Total" etiketinin metnini alır.

```csharp
public override string GetTextOfGrandTotal()
```

### Dönüş Değeri

"Grand Total" etiketinin metni

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur (sadece bağlam için)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // SettablePivotGlobalizationSettings örneği
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Varsayılan "Grand Total" metnini değiştirin
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Mevcut "Grand Total" metnini alın
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Çalışma kitabını kaydedin (pivot tablo oluşturulmaz, ancak dosya kaydedilir ve çalıştırma kanıtlanır)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


