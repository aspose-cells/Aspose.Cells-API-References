---
title: "LegendEntry.Background"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LegendEntry. Ottiene e imposta la modalità di visualizzazione dello sfondo"
type: docs
url: /it/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Ottiene e imposta la modalità di visualizzazione dello sfondo

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà LegendEntry.BackgroundMode. Questa proprietà sarà rimossa 12 mesi dopo a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Ottieni la prima voce della legenda
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // Visualizza il valore corrente della proprietà Background
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // Imposta un nuovo valore per Background (poiché non è di sola lettura)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // Imposta un altro valore per Background
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // Salva la cartella di lavoro
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
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

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


