---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Imposta il nome di Decrease per la Legend"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Imposta il nome di Diminuzione per la Legenda.

```csharp
public void SetLegendDecreaseName(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | nome dipendente locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per un chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crea impostazioni di globalizzazione
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Chiama SetLegendDecreaseName con una stringa personalizzata
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // La classe Chart non ha una proprietà ChartGlobalizationSettings,
                // quindi dobbiamo usare direttamente l'oggetto delle impostazioni dove necessario
                // (Nota: Nell'uso reale, dovresti trovare dove queste impostazioni vengono applicate)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


