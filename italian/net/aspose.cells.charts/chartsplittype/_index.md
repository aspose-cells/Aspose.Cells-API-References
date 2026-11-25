---
title: "Enum ChartSplitType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ChartSplitType enum. Rappresenta il modo in cui le due sezioni di un grafico a torta di torta o di un grafico a barra di torta sono suddivise"
type: docs
url: /it/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Rappresenta il modo in cui le due sezioni di un grafico a torta di torta o a barra di torta sono suddivise.

```csharp
public enum ChartSplitType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Position | `0` | Rappresenta i punti dati. I punti dati devono essere suddivisi tra la torta e il secondo grafico posizionando l'ultima posizione di divisione dei punti dati nel secondo grafico. |
| Value | `1` | Rappresenta i punti dati che devono essere suddivisi tra la torta e il secondo grafico posizionando i punti dati con valore inferiore a Posizione di divisione nel secondo grafico. |
| PercentValue | `2` | Rappresenta i punti dati che devono essere suddivisi tra la torta e il secondo grafico posizionando i punti con una percentuale inferiore alla percentuale di Posizione di divisione nel secondo grafico. |
| Custom | `3` | Rappresenta i punti dati che devono essere suddivisi tra la torta e il secondo grafico secondo i valori di divisione personalizzata. |
| Auto | `4` | Rappresenta i punti dati che devono essere suddivisi utilizzando il meccanismo predefinito per questo tipo di grafico. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio per il grafico
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Aggiungi un grafico a torta
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Imposta l'intervallo dati del grafico
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Mostra i diversi valori di ChartSplitType
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Cambia a un altro tipo di divisione
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Salva la cartella di lavoro
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


