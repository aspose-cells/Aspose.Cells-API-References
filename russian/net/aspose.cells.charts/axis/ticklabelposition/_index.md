---
title: "Axis.TickLabelPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет положение меток делений на указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Представляет положение меток делений на указанной оси.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить положение метки деления
            chart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            
            // Сохраните книгу
            workbook.Save("AxisPropertyTickLabelPositionDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


