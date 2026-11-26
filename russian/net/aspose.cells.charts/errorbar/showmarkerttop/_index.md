---
title: "ErrorBar.ShowMarkerTTop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ErrorBar. Указывает, применяется ли форматирование полос ошибок с Ttop"
type: docs
url: /ru/net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Указывает, следует ли форматировать полосы ошибок с верхушкой‑Т.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyShowMarkerTTopDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(2);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(1);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите данные диаграммы
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Настроить полосы ошибок для первой серии
            Series series = chart.NSeries[0];
            series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
            series.YErrorBar.Type = ErrorBarType.Percent;
            series.YErrorBar.Amount = 10;
            
            // Продемонстрировать свойство ShowMarkerTTop
            series.YErrorBar.ShowMarkerTTop = true;
            series.YErrorBar.Color = System.Drawing.Color.Red;
            series.YErrorBar.Style = LineType.DashDot;

            // Сохраните книгу
            workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


