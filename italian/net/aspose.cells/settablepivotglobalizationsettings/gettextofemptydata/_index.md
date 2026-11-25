---
title: "SettablePivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta vuota nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

Restituisce il testo dell'etichetta "(blank)" nella PivotTable.

```csharp
public override string GetTextOfEmptyData()
```

### Valore di ritorno

Il testo dei dati vuoti

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ottieni il testo predefinito per i dati vuoti
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // Imposta un testo personalizzato per i dati vuoti
                settings.SetTextOfEmptyData("No Data Available");

                // Ottieni il testo aggiornato per i dati vuoti
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // Applica le impostazioni alla cartella di lavoro
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


