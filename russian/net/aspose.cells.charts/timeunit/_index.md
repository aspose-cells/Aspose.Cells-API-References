---
title: "Перечисление TimeUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.TimeUnit enum. Представляет базовую единицу для оси категорий"
type: docs
url: /ru/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Представляет базовую единицу для оси категорий.

```csharp
public enum TimeUnit
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Days | `0` | Дни |
| Months | `1` | Месяцы |
| Years | `2` | Годы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Добавить новый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию к диаграмме
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Установить ось категорий для использования единиц времени
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Настроить внешний вид диаграммы
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Сохраните книгу
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


