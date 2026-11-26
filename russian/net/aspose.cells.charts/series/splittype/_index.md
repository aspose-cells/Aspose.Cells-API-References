---
title: "Series.SplitType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает или задает значение, определяющее, какие точки данных находятся во второй части круговой диаграммы (pie of pie) или столбце (bar of pie) диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Возвращает или задает значение, определяющее, какие точки данных находятся во второй части (круге или полосе) диаграммы «круг в круге» или «полоска в круге».

```csharp
public ChartSplitType SplitType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавить круговую диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить тип разделения для первой серии
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Сохраните книгу
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


