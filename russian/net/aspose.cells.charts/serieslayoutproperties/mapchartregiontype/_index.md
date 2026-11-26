---
title: "SeriesLayoutProperties.MapChartRegionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesLayoutProperties. Получает и задает тип региона карты"
type: docs
url: /ru/net/aspose.cells.charts/serieslayoutproperties/mapchartregiontype/
---
## SeriesLayoutProperties.MapChartRegionType property

Получает и задает тип региона карты.

```csharp
public MapChartRegionType MapChartRegionType { get; set; }
```

### Примечания

Только для картографической диаграммы.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapChartRegionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            workbook.Save("MapChartRegionTypeExample.xlsx");
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### См. также

* enum [MapChartRegionType](../../mapchartregiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


