---
title: "ErrorBar.MinusValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ErrorBar. Представляет отрицательное значение ошибки, когда тип полосы ошибок — Custom"
type: docs
url: /ru/net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Представляет отрицательную величину ошибки, когда тип полосы ошибок установлен как Custom.

```csharp
public string MinusValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyMinusValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(15);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию
            chart.NSeries.Add("B2:B3", true);

            // Настроить полосы ошибок
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";
            errorBar.MinusValue = "=A3";

            // Сохраните книгу
            workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


