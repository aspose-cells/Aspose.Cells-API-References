---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesLayoutProperties. Указывает, отображаются ли маркеры, обозначающие среднее"
type: docs
url: /ru/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Указывает, отображаются ли маркеры, обозначающие среднее.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Создать диаграмму (используя тип Column, который поддерживает маркеры среднего)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // Настроить свойства макета с помощью ShowMeanMarker
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Сохранить результат
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### См. также

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


