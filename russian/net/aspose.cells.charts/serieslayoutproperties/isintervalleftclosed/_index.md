---
title: "SeriesLayoutProperties.IsIntervalLeftClosed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesLayoutProperties. Указывает, закрыт ли интервал с левой стороны"
type: docs
url: /ru/net/aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/
---
## SeriesLayoutProperties.IsIntervalLeftClosed property

Указывает, закрыт ли интервал с левой стороны.

```csharp
public bool IsIntervalLeftClosed { get; set; }
```

### Примечания

Только для диаграммы ParetoLine.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Установить свойство IsIntervalLeftClosed
            series.LayoutProperties.IsIntervalLeftClosed = true;

            // Сохранить книгу
            workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


