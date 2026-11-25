---
title: "Enum MapChartLabelLayout"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.MapChartLabelLayout. Rappresenta il layout delle etichette dei grafici cartografici"
type: docs
url: /it/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Rappresenta il layout delle etichette del grafico mappa.

```csharp
public enum MapChartLabelLayout
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| BestFitOnly | `0` | Viene utilizzata solo la migliore corrispondenza. |
| ShowAll | `1` | Mostra tutte le etichette. |
| None | `2` | Non ci sono etichette. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico cartografico
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Aggiungi un grafico mappa al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo di dati per il grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle proprietà di layout della serie
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Imposta il layout delle etichette del grafico cartografico
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Salva la cartella di lavoro
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


