---
title: "Line.BeginType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает наконечник стрелки для начала линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Указывает наконечник стрелки для начала линии.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Добавить линейную диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("A1:A3", true);

            // Получите первую серию и настройте её свойства линии
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Сохраните книгу
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


