---
title: "SettableChartGlobalizationSettings.SetAxisUnitName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il Nome dell'Unità dell'Asse"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

Imposta il nome dell'Unità dell'Asse.

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | DisplayUnitType | Il tipo di unità per la visualizzazione delle etichette dell'asse. |
| name | String | nome dipendente locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati minimi per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta nomi personalizzati delle unità dell'asse per diversi tipi di unità di visualizzazione
                settings.SetAxisUnitName(DisplayUnitType.Thousands, "K");
                settings.SetAxisUnitName(DisplayUnitType.Millions, "M");
                settings.SetAxisUnitName(DisplayUnitType.Percentage, "Pct");

                // Verifica le impostazioni recuperando i valori
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Visualizza i risultati
                Console.WriteLine($"Thousands unit name set to: {thousandsUnit}");
                Console.WriteLine($"Millions unit name set to: {millionsUnit}");
                Console.WriteLine($"Percentage unit name set to: {percentageUnit}");

                // Salva la cartella di lavoro
                workbook.Save("SetAxisUnitNameDemo.xlsx");
                Console.WriteLine("SetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


