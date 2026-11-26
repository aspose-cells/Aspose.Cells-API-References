---
title: "Перечисление MapChartProjectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.MapChartProjectionType. Представляет тип проекции картовой диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

Представляет тип проекции карты диаграммы.

```csharp
public enum MapChartProjectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Автоматически |
| Mercator | `1` | Меркатор |
| Miller | `2` | Миллер |
| Albers | `3` | Алберса |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные в лист для картовой диаграммы
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Добавьте картовую диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Установите тип проекции для картовой диаграммы
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Выведите тип проекции
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Сохраните книгу
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


