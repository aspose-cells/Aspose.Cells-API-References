---
title: "SettableChartGlobalizationSettings.SetLegendIncreaseName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome di increase per la Legenda"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Imposta il nome di Aumento per la Legenda.

```csharp
public void SetLegendIncreaseName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati minimi per il contesto
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta un nome personalizzato per l'incremento della legenda
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Verifica l'impostazione ottenendo il valore
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Salva la cartella di lavoro
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


