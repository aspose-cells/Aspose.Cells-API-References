---
title: "TickLabels.Number"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Представляет номер формата для объекта TickLabels"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Представляет номер формата для объекта TickLabels.

```csharp
public int Number { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Настройте подписи делений
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Сохраните книгу
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


