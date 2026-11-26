---
title: "Series.SecondPlotSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Возвращает или задает размер вторичной секции либо диаграммы pie of pie, либо bar of pie в виде процента от размера основной диаграммы. Может принимать значение от 5 до 200"
type: docs
url: /ru/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Возвращает или задает размер вторичной части либо диаграммы «круг в круге», либо «полоска в круге», в процентах от размера основного круга. Может принимать значение от 5 до 200.

```csharp
public short SecondPlotSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы pie.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию
            Series series = chart.NSeries[0];

            // Установите свойство SecondPlotSize (процент диаграммы, отображаемый во втором графике)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Сохраните книгу
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


