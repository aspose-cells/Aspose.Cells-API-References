---
title: "ErrorBar.PlusValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ErrorBar. Представляет положительное значение ошибки, когда тип полосы ошибок — Custom"
type: docs
url: /ru/net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Представляет положительную величину ошибки, когда тип полосы ошибок установлен как Custom.

```csharp
public string PlusValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyPlusValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);

            // Настроить полосы ошибок
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";  // Using PlusValue property
            errorBar.MinusValue = "=A3";

            // Сохраните книгу
            workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


