---
title: "SettableChartGlobalizationSettings.GetAxisUnitName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableChartGlobalizationSettings yöntemi. Eksen biriminin adını alır"
type: docs
url: /tr/net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

Eksen biriminin adını alır.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için minimum veri ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // SettableChartGlobalizationSettings örneği oluştur
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Farklı DisplayUnitType değerleriyle GetAxisUnitName'i çağırın
                string hundredsUnit = settings.GetAxisUnitName(DisplayUnitType.Hundreds);
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Sonuçları görüntüleyin
                Console.WriteLine($"Hundreds unit name: {hundredsUnit}");
                Console.WriteLine($"Thousands unit name: {thousandsUnit}");
                Console.WriteLine($"Millions unit name: {millionsUnit}");
                Console.WriteLine($"Percentage unit name: {percentageUnit}");

                // Çalışma kitabını kaydedin
                workbook.Save("GetAxisUnitNameDemo.xlsx");
                Console.WriteLine("GetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


