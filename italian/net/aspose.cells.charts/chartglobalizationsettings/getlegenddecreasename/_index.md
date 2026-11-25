---
title: "ChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartGlobalizationSettings. Ottiene il nome della Diminuzione per la Legenda"
type: docs
url: /it/net/aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/
---
## ChartGlobalizationSettings.GetLegendDecreaseName method

Ottiene il nome di Diminuzione per la Legenda.

```csharp
public virtual string GetLegendDecreaseName()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crea le impostazioni di globalizzazione e ottieni il nome della diminuzione della legenda
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();

            // Restituisci il risultato
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

            // Salva la cartella di lavoro
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


