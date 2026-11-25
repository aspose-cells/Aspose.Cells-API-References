---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo localizzato di tutti i periodi"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

Ottiene il testo localizzato di "All Periods".

```csharp
public virtual string GetTextOfAllPeriods()
```

### Esempi

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
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio per creare il contesto per la tabella pivot
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Crea un'istanza di PivotGlobalizationSettings
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // Dimostra il metodo GetTextOfAllPeriods
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // Mostra le etichette dei periodi di tempo correlati per il contesto
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // Salva la cartella di lavoro
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

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


