---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metod. Hämtar den lokaliserade texten för All Periods"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

Hämtar den lokaliserade texten för "All Periods".

```csharp
public virtual string GetTextOfAllPeriods()
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata för att skapa kontext för pivottabell
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Skapa en PivotGlobalizationSettings‑instans
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // Demonstrera GetTextOfAllPeriods‑metoden
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // Visa relaterade tidsperiodetiketter för kontext
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // Spara arbetsboken
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

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


