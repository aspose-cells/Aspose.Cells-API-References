---
title: "Enum MapChartProjectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.MapChartProjectionType enum. Rappresenta il tipo di proiezione del grafico mappa"
type: docs
url: /it/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

Rappresenta il tipo di proiezione del grafico mappa.

```csharp
public enum MapChartProjectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Automatico |
| Mercator | `1` | Mercatore |
| Miller | `2` | Miller |
| Albers | `3` | Albers |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartProjectionTypeDemo
    {
        public static void MapChartProjectionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro per il grafico mappa
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Aggiungi un grafico mappa al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il tipo di proiezione per il grafico mappa
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Restituisci il tipo di proiezione
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Salva la cartella di lavoro
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


