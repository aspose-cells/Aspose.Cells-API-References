---
title: "TickLabels.DirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Получает и задает направление текста"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Получает и задает направление текста.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = 50;
            worksheet.Cells["A2"].Value = 100;
            worksheet.Cells["A3"].Value = 150;
            worksheet.Cells["A4"].Value = 200;
            worksheet.Cells["B1"].Value = 60;
            worksheet.Cells["B2"].Value = 32;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 40;
            worksheet.Cells["C1"].Value = "清华";
            worksheet.Cells["C2"].Value = "北大";
            worksheet.Cells["C3"].Value = "人大";
            worksheet.Cells["C4"].Value = "科大";

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите данные диаграммы
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Установить вертикальное направление меток делений
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;

            // Сохраните книгу
            workbook.Save("TickLabelsDirectionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


