---
title: "Enum PlotDataByType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.PlotDataByType enum. Rappresenta il tipo di tracciamento dei dati per riga o colonna"
type: docs
url: /it/net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Rappresenta il tipo di tracciamento dei dati per riga o colonna.

```csharp
public enum PlotDataByType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Row | `0` | Ordinato per riga. |
| Column | `1` | Per colonna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Aggiungi un grafico al foglio di lavoro
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Imposta l'intervallo dati del grafico
                chart.NSeries.Add("B2:C3", true);

                // Dimostrazione dell'uso dei valori dell'enum PlotDataByType
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Cambia a tracciamento per colonna
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Salva la cartella di lavoro
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


