---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il nome di increase per la Legenda"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Ottiene il nome di Aumento per la Legenda.

```csharp
public override string GetLegendIncreaseName()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
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

                // Imposta un nome personalizzato per l'incremento della legenda
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Ottieni il nome dell'incremento della legenda usando GetLegendIncreaseName
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // Salva la cartella di lavoro
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


