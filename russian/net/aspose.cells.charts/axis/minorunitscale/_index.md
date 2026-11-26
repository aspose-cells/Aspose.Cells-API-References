---
title: "Axis.MinorUnitScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет масштаб основной единицы для категориальной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/minorunitscale/
---
## Axis.MinorUnitScale property

Представляет масштаб основной единицы для оси категорий.

```csharp
public TimeUnit MinorUnitScale { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример данных, основанных на времени
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
                worksheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Настроить ось категорий как временную шкалу
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Сохраните книгу
            workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


