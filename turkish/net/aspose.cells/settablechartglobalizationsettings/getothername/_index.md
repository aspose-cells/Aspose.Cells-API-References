---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Grafik için Other etiketlerinin adını alır"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Grafik için "Other" etiketlerinin adını alır.

```csharp
public override string GetOtherName()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Minimum veri ekle (isteğe bağlı, sadece tam bir çalışma kitabı için)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Küreselleştirme ayarları nesnesini örnekle
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // "Other" etiketi için özel bir ad ayarla
                settings.SetOtherName("Custom Other Label");

                // GetOtherName kullanarak adı al
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Çalışma kitabını kaydet (ayarlar bu demoda doğrudan grafiğe eklenmemiştir)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


