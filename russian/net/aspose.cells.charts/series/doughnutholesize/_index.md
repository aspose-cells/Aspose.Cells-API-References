---
title: "Series.DoughnutHoleSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Возвращает или задает размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы в диапазоне от 10 до 90 процентов"
type: docs
url: /ru/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Возвращает или задает размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы, от 10 до 90 процентов.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить диаграмму Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите размер отверстия кольца (процент от радиуса диаграммы)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Сохраните книгу
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


