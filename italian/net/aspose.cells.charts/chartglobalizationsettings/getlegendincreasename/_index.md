---
title: "ChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartGlobalizationSettings. Ottiene il nome dell'aumento per la Legenda"
type: docs
url: /it/net/aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/
---
## ChartGlobalizationSettings.GetLegendIncreaseName method

Ottiene il nome di Aumento per la Legenda.

```csharp
public virtual string GetLegendIncreaseName()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico di esempio
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crea le impostazioni di globalizzazione e ottieni il nome dell'aumento della legenda
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();

            // Restituisci il risultato
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

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


