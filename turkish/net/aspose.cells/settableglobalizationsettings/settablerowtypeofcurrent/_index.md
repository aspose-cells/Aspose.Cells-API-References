---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Referans verilen tabloda mevcut satırı içeren tablo satırlarının tip adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tür adını ayarlar.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluştur
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Küreselleştirme ayarları oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Mevcut satır tipi için özel bir ad ayarlayın
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                // Değeri geri alarak ayarı doğrulayın
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Çalışma kitabını kaydedin
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


