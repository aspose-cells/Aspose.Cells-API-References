---
title: "Trendline.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Возвращает тип трендовой линии"
type: docs
url: /ru/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Возвращает тип линии тренда.

```csharp
public TrendlineType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Добавить серию
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Добавьте экспоненциальную трендовую линию
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Сохраните книгу
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


