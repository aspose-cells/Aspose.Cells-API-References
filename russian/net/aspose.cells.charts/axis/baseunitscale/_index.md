---
title: "Axis.BaseUnitScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет масштаб базовой единицы для категориальной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Представляет масштаб базовой единицы для оси категорий.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Примечания

Действует только когда свойство CategoryType установлено в TimeScale.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Установите масштаб базовой единицы для категориальной оси
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Сохраните книгу
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


