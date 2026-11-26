---
title: "Series.UpBars"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает объект DropBars, представляющий верхние бары на линейной диаграмме. Применяется только к линейным диаграммам"
type: docs
url: /ru/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Возвращает объект DropBars, представляющий верхние бары на линейной диаграмме. Применяется только к линейным диаграммам.

```csharp
public DropBars UpBars { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyUpBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных для линейной диаграммы с верхними/нижними барами
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Включите и настройте верхние бары
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### См. также

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


