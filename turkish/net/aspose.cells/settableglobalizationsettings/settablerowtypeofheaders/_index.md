---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Tablo başlığını içeren tablo satırlarının tür adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Tablo başlığını içeren tablo satırlarının tür adını ayarlar.

```csharp
public void SetTableRowTypeOfHeaders(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | tablo satırlarının tip adı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluştur ve bazı veriler ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Bir ListObject (Tablo) oluştur
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // SetTableRowTypeOfHeaders yöntemini özel başlık tür adıyla çağır
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


