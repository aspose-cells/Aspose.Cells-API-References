---
title: "Series.IsColorVaried"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет, изменяется ли цвет точек. Диаграмма должна содержать только одну серию или быть круговой диаграммой."
type: docs
url: /ru/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Представляет, варьируется ли цвет точек. Диаграмма должна содержать только одну серию или быть круговой диаграммой.

```csharp
public bool IsColorVaried { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить свойство IsColorVaried для первой серии
            chart.NSeries[0].IsColorVaried = true;

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверить свойство
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


