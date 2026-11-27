---
title: "Enum MapChartLabelLayout"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.MapChartLabelLayout enum. Representerar layouten för kartdiagrammets etiketter"
type: docs
url: /sv/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Representerar layouten för kartdiagrammets etiketter.

```csharp
public enum MapChartLabelLayout
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| BestFitOnly | `0` | Endast den bästa passformen används. |
| ShowAll | `1` | Visar alla etiketter. |
| None | `2` | Det finns inga etiketter. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för kartdiagrammet
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Lägg till ett kartdiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till seriens layoutegenskaper
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Ställ in layouten för kartdiagrammets etiketter
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Spara arbetsboken
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


