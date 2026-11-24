---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings Methode. Gibt den lokalisierten Text aller Perioden zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

Ruft den lokalisierten Text von "All Periods" ab.

```csharp
public virtual string GetTextOfAllPeriods()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOfAllPeriodsDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Beispieldaten hinzufügen, um Kontext für die Pivot-Tabelle zu erstellen
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // Pivot-Tabelle erstellen
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // PivotGlobalizationSettings-Instanz erstellen
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // Demonstriere die GetTextOfAllPeriods-Methode
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // Verwandte Zeitperiodenbeschriftungen für den Kontext anzeigen
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // Speichere die Arbeitsmappe
                workbook.Save("GetTextOfAllPeriodsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


