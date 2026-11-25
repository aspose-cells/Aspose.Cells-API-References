---
title: "Series.DisplayName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene il nome della serie che viene visualizzato sul grafico."
type: docs
url: /it/net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Ottiene il nome della serie visualizzato sul grafico.

```csharp
public string DisplayName { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Accedi alla prima serie e visualizza il suo DisplayName
                Series series = chart.NSeries[0];
                Console.WriteLine("Series DisplayName: " + series.DisplayName);

                // Mostra anche la proprietà Name per confronto
                Console.WriteLine("Series Name: " + series.Name);

                // Salva la cartella di lavoro
                workbook.Save("DisplayNameDemo.xlsx");
                Console.WriteLine("DisplayName has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


