---
title: "ChartTextFrame.TextDirection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Представляет порядок чтения текста"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Представляет порядок чтения текста.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ChartTextFrame.ReadingOrder. Это свойство будет удалено через 12 месяцев, начиная с марта 2020 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Настройте данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настройте подписи данных
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            
            // Продемонстрировать свойство TextDirection
            dataLabels.TextDirection = TextDirectionType.LeftToRight;

            // Сохраните книгу
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


