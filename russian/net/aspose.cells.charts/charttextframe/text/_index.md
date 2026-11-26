---
title: "ChartTextFrame.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Получает или задает текст заголовка фрейма"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Получает или задает текст заголовка рамки.

```csharp
public virtual string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Установить текст заголовка диаграммы
            chart.Title.Text = "Sample Chart Title";

            // Получить доступ и изменить текст легенды
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Сохраните книгу
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


