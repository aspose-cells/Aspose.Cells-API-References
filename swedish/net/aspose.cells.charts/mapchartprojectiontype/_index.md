---
title: "Enum MapChartProjectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.MapChartProjectionType enum. Representerar projektionstypen för kartdiagrammet"
type: docs
url: /sv/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

Representerar projektionstypen för kartdiagrammet.

```csharp
public enum MapChartProjectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Automatisk |
| Mercator | `1` | Mercator |
| Miller | `2` | Miller |
| Albers | `3` | Albers |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet för kartdiagrammet
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Lägg till ett kartdiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Ställ in projektionstypen för kartdiagrammet
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Skriv ut projektionstypen
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Spara arbetsboken
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


