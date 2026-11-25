---
title: "Enum MapChartRegionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.MapChartRegionType enum. Rappresenta il tipo di regione del grafico mappa"
type: docs
url: /it/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

Rappresenta il tipo di regione del grafico mappa.

```csharp
public enum MapChartRegionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Automatico |
| DataOnly | `1` | Contiene solo dati. |
| CountryRegionList | `2` | Elenco delle regioni dei paesi. |
| World | `3` | Mondo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartRegionTypeDemo
    {
        public static void MapChartRegionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi un grafico mappa al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il tipo di regione del grafico mappa
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Salva la cartella di lavoro
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Restituisci il risultato
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


