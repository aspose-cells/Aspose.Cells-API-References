---
title: "Series.SplitValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает или задаёт значение, которое будет использоваться для определения, какие точки данных находятся во втором секторе или столбце на диаграмме «круг в круге» или «столбец в круге»"
type: docs
url: /ru/net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во второй части (круге или полосе) диаграммы «круг в круге» или «полоска в круге».

```csharp
public double SplitValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);
            worksheet.Cells["B5"].PutValue(50);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Установите тип разбиения и значение
            chart.NSeries[0].SplitType = ChartSplitType.Custom;
            chart.NSeries[0].SplitValue = 20; // Split points with value <= 20

            // Сохраните книгу
            workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


