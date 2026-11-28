---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. PivotTable'daki Toplam etiketi metnini alır. Veri alanında iki veya daha fazla PivotField bulunduğunda bu yöntemi geçersiz kılmanız gerekir."
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

PivotTable'daki "Total" etiketinin metnini alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir.

```csharp
public override string GetTextOfTotal()
```

### Dönüş Değeri

"Total" etiketinin metni

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // SettablePivotGlobalizationSettings bir örnek oluştur
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // "Total" etiketi için özel metin ayarla
                settings.SetTextOfTotal("Custom Total");

                // "Total" etiketinin metnini al
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // Çalışma kitabını kaydedin
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


