---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il nome del Titolo del Grafico"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Ottiene il nome del Titolo del Grafico.

```csharp
public override string GetChartTitleName()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Imposta un nome personalizzato per il titolo del grafico
                settings.SetChartTitleName("Custom Chart Title");

                // Ottieni il nome del titolo del grafico usando GetChartTitleName
                string chartTitleName = settings.GetChartTitleName();

                // Visualizza il risultato
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Salva la cartella di lavoro
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


