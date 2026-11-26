---
title: "Series.Points"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает коллекцию точек в серии на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/points/
---
## Series.Points property

Получает коллекцию точек в ряду диаграммы.

```csharp
public ChartPointCollection Points { get; }
```

### Примечания

Когда диаграмма является «Круг в круге» или «Бар в круге», последняя точка является точкой «другое» в первом круге.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
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
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к первой серии и её точкам
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Добавьте подписи данных к каждой точке
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Сохраните книгу
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


