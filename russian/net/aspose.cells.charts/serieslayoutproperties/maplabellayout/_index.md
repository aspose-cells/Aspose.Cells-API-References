---
title: "SeriesLayoutProperties.MapLabelLayout"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesLayoutProperties. Получает и задает макет меток карты"
type: docs
url: /ru/net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

Получает и задает расположение меток карты.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы карты
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("United States");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B4"].PutValue(60);

            // Добавить диаграмму карты
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[0];
            series.XValues = "A2:A4";

            // Настроить свойства макета карты
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            // Сохраните книгу
            workbook.Save("MapLabelLayoutDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


