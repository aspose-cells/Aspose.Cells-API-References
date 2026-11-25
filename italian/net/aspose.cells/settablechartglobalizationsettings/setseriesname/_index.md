---
title: "SettableChartGlobalizationSettings.SetSeriesName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome della Serie nel Grafico"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Imposta il nome della Serie nel Grafico

```csharp
public void SetSeriesName(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | nome dipendente locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
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

                // Imposta un nome di serie personalizzato usando SetSeriesName con un parametro stringa
                settings.SetSeriesName("Custom Series Label");

                // Verifica l'impostazione ottenendo il nome della serie
                string seriesName = settings.GetSeriesName();
                Console.WriteLine($"Series name set to: {seriesName}");

                // Salva la cartella di lavoro
                workbook.Save("SetSeriesNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetSeriesName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


