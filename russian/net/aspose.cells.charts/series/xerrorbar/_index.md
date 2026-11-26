---
title: "Series.XErrorBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет ошибочную полосу по оси X серии"
type: docs
url: /ru/net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Представляет ошибочную полосу по направлению X ряда.

```csharp
public ErrorBar XErrorBar { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXErrorBarDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию, используя данные
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            Series series = seriesCollection[0];
            series.XValues = "A2:A4";

            // Настройте свойства XErrorBar
            series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
            series.XErrorBar.Amount = 0.5;
            series.XErrorBar.Type = ErrorBarType.FixedValue;

            // Сохраните книгу
            workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


