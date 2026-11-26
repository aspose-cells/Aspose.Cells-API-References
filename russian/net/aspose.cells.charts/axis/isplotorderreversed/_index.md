---
title: "Axis.IsPlotOrderReversed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает, строит ли Microsoft Excel точки данных от последней к первой"
type: docs
url: /ru/net/aspose.cells.charts/axis/isplotorderreversed/
---
## Axis.IsPlotOrderReversed property

Представляет, строит ли Microsoft Excel точки данных от последней к первой.

```csharp
public bool IsPlotOrderReversed { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsPlotOrderReversedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Обратить порядок построения категорий
            chart.CategoryAxis.IsPlotOrderReversed = true;

            // Сохраните книгу
            workbook.Save("AxisPropertyIsPlotOrderReversedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


