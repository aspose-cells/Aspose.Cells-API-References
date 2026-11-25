---
title: "SettableChartGlobalizationSettings.SetLegendTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome di Total per la Legenda"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

Imposta il nome di Totale per la Legenda.

```csharp
public void SetLegendTotalName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati minimi per il contesto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Crea un'istanza di SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Imposta un nome personalizzato per il totale della legenda
                settings.SetLegendTotalName("Custom Total Label");

                // Verifica l'impostazione ottenendo il valore
                string legendTotalName = settings.GetLegendTotalName();
                Console.WriteLine("Legend Total Name set to: " + legendTotalName);

                // Salva la cartella di lavoro
                workbook.Save("SetLegendTotalNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


