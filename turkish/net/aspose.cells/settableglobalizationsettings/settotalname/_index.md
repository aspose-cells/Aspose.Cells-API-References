---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Belirli bir işlevin toplam adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

Belirli işlevin toplam adını ayarlar.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | ConsolidationFunction | İşlev tipi. |
| name | String | İşlevin toplam adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Konsolidasyon için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Sum işlevi için özel toplam ad ayarla
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // Ortalama işlevi için özel toplam adını ayarla
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                // Ayarları, değerleri geri alarak doğrula
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // Etkiyi göstermek için bir pivot tablo oluştur
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Çalışma kitabını kaydedin
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


