---
title: "SeriesCollection.ChangeColors"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Imposta una palette monocromatica per le serie del grafico"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Imposta la palette monocromatica per le serie del grafico.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ChartColorPaletteType | Il tipo monocromatico. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Popola alcuni dati per il grafico
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Aggiungi un grafico a colonne
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Imposta l'intervallo di dati per la serie
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la raccolta di serie
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Modifica la tavolozza dei colori di tutte le serie nella raccolta.
                // Usa un cast numerico a un valore enum valido (ad es., 0) per evitare i nomi dei membri enum dipendenti.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Salva la cartella di lavoro per verificare il risultato
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


