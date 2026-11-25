---
title: "SettableChartGlobalizationSettings.GetSeriesName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableChartGlobalizationSettings. Ottiene il nome della Serie nel Chart"
type: docs
url: /it/net/aspose.cells/settablechartglobalizationsettings/getseriesname/
---
## SettableChartGlobalizationSettings.GetSeriesName method

Ottiene il nome della Serie nel Grafico.

```csharp
public override string GetSeriesName()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Column A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Column B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crea e applica le impostazioni di globalizzazione
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetSeriesName("Custom Series Name");
            
            // Le impostazioni di globalizzazione sono usate durante il rendering/visualizzazione del chart,
            // ma non sono assegnate direttamente all'oggetto chart
            // (poiché la classe Chart non ha questa proprietà)

            try
            {
                // Ottieni il nome della serie personalizzata
                string seriesName = settings.GetSeriesName();
                Console.WriteLine("Series Name: " + seriesName);

                // Salva la cartella di lavoro
                workbook.Save("MethodGetSeriesNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


