---
title: "Enum MapChartRegionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.MapChartRegionType enum. Representerar regiontypen för kartdiagrammet"
type: docs
url: /sv/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

Representerar regionstypen för kartdiagrammet.

```csharp
public enum MapChartRegionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Automatisk |
| DataOnly | `1` | Innehåller endast data. |
| CountryRegionList | `2` | Lista över landsregioner. |
| World | `3` | Världen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till ett kartdiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Ställ in regiontypen för kartdiagrammet
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Spara arbetsboken
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Skriv ut resultatet
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


