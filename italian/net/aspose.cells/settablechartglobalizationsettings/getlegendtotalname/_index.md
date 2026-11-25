---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il nome del Totale per la Legenda"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Ottiene il nome di Totale per la Legenda.

```csharp
public override string GetLegendTotalName()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta prima un nome personalizzato per il totale della legenda
                settings.SetLegendTotalName("Custom Total Label");

                // Chiama il metodo GetLegendTotalName per recuperare il valore
                string legendTotalName = settings.GetLegendTotalName();

                // Visualizza il risultato
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Salva la cartella di lavoro
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


