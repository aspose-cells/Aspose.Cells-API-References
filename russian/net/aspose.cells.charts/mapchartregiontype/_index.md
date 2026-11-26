---
title: "Перечисление MapChartRegionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.MapChartRegionType. Представляет тип региона карты диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

Представляет тип региона карты диаграммы.

```csharp
public enum MapChartRegionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Автоматически |
| DataOnly | `1` | Содержит только данные. |
| CountryRegionList | `2` | Список регионов страны. |
| World | `3` | Мир. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Добавьте картовую диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Установить тип региона карты диаграммы
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Сохраните книгу
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Вывести результат.
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


