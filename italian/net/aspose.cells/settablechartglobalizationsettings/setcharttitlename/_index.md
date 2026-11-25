---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome del titolo del grafico"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

Imposta il nome del Titolo del Grafico.

```csharp
public void SetChartTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // Chiama SetChartTitleName con una stringa personalizzata
                settings.SetChartTitleName("Custom Chart Title");

                // Verifica l'impostazione ottenendo il valore
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // Salva la cartella di lavoro
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


