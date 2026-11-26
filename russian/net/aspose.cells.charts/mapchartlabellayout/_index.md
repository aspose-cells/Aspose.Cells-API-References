---
title: "Перечисление MapChartLabelLayout"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.MapChartLabelLayout. Представляет расположение меток карт"
type: docs
url: /ru/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Представляет макет подписей карты диаграммы.

```csharp
public enum MapChartLabelLayout
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| BestFitOnly | `0` | Используется только наилучшее соответствие. |
| ShowAll | `1` | Показывает все метки. |
| None | `2` | Нет меток. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для картографической диаграммы
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Добавьте картовую диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к свойствам макета серии
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Установить расположение меток картографической диаграммы
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Сохраните книгу
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


