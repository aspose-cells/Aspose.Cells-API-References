---
title: "TickLabels.ReadingOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Представляет порядок чтения текста"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Представляет порядок чтения текста.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Установить порядок чтения меток делений
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Сохраните книгу
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


