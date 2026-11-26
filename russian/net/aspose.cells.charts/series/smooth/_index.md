---
title: "Series.Smooth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Представляет сглаживание кривой. True, если сглаживание включено для линейной диаграммы или диаграммы разброса. Применяется только к линейным диаграммам и диаграммам разброса с линиями"
type: docs
url: /ru/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Представляет сглаживание кривой. Истина, если сглаживание включено для линейной диаграммы или диаграммы разброса. Применяется только к линейным диаграммам и диаграммам разброса с линиями.

```csharp
public bool Smooth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите свойство Smooth для первой серии
            chart.NSeries[0].Smooth = true;

            // Сохраните книгу
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


