---
title: "ErrorBar.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ErrorBar. Представляет тип величины полосы ошибок"
type: docs
url: /ru/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Представляет тип величины полосы ошибок.

```csharp
public ErrorBarType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавьте примерные данные
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Создать диаграмму
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Добавить данные серии
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Установить пользовательский тип полосы ошибок и значения
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Сохраните книгу
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


