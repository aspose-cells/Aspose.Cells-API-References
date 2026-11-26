---
title: "Series.HasSeriesLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Истина, если у сложенной столбчатой диаграммы или гистограммы есть линии серии, или если у диаграммы «Круг в круге» или «Бар в круге» есть соединительные линии между двумя секциями. Применяется только к сложенным столбчатым диаграммам, гистограммам, диаграммам «Круг в круге» или «Бар в круге»"
type: docs
url: /ru/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

Истина, если у сложенной столбчатой или гистограммы есть линии серии, или если у диаграммы «Круг в круге» или «Бар в круге» есть соединительные линии между двумя секциями. Применяется только к сложенным столбчатым диаграммам, гистограммам, диаграммам «Круг в круге» и «Бар в круге».

```csharp
public bool HasSeriesLines { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Добавить сложенную столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить данные серии
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Получить доступ к первой серии
            Series series = chart.NSeries[0];
            
            // Продемонстрировать свойство HasSeriesLines
            series.HasSeriesLines = true; // Enable series lines
            
            // Сохраните книгу
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


