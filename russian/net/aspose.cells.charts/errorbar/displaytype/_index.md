---
title: "ErrorBar.DisplayType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ErrorBar. Представляет тип отображения полосы ошибок"
type: docs
url: /ru/net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Представляет тип отображения полосы ошибок.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyDisplayTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Установить тип отображения полосы ошибок
            chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

            // Сохраните книгу
            workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


