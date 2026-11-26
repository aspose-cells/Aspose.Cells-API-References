---
title: "Axis.MajorTickMark"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет тип основной метки деления для указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Представляет тип основных делений для указанной оси.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить тип основной метки деления наружу
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Сохраните книгу
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


