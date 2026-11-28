---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettablePivotGlobalizationSettings yöntemi. Belirtilen korumalı ad için metni alır"
type: docs
url: /tr/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Belirtilen korumalı ad için metni alır.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectedName | String | PivotTable'daki korumalı ad. |

### Dönüş Değeri

PivotTable'ın yerel korumalı adları.

### Açıklamalar

Ms Excel'de, bazı adların PivotTable'da PivotFields adı olarak kullanılması izin verilmez. Bunlar bölgeye göre farklılık gösterir, kullanıcı kullanılan bölgeye göre bunları açıkça belirtebilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // SettablePivotGlobalizationSettings bir örnek oluştur
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Korumalı bir ad için özel metin ayarla
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Korumalı adın metnini al
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Çalışma kitabını kaydedin
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


