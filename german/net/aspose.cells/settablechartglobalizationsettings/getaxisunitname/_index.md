---
title: "SettableChartGlobalizationSettings.GetAxisUnitName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Gibt den Namen der Achseneinheit zurück"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

Liefert den Namen der Achseneinheit.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie minimale Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Rufen Sie GetAxisUnitName mit verschiedenen DisplayUnitType-Werten auf
                string hundredsUnit = settings.GetAxisUnitName(DisplayUnitType.Hundreds);
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Ergebnisse anzeigen
                Console.WriteLine($"Hundreds unit name: {hundredsUnit}");
                Console.WriteLine($"Thousands unit name: {thousandsUnit}");
                Console.WriteLine($"Millions unit name: {millionsUnit}");
                Console.WriteLine($"Percentage unit name: {percentageUnit}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


