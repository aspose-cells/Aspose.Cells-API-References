---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Referans verilen tablonun veri bölgesinden oluşan tablo satırlarının tip adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Referans alınan tablonun veri bölgesini içeren tablo satırlarının tür adını ayarlar.

```csharp
public void SetTableRowTypeOfData(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluştur
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Küreselleştirme ayarları oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Tablodaki veri satırları için özel ad ayarlayın
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


