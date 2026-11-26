---
title: "Legend.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Legend. Получает или задает тип положения легенды"
type: docs
url: /ru/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Получает или задает тип положения легенды.

```csharp
public LegendPositionType Position { get; set; }
```

### Примечания

Позиция по умолчанию — справа. Если легенда находится слева или справа от диаграммы, установка свойства Legend.X не будет иметь эффекта. Если легенда находится сверху или снизу диаграммы, установка свойства Legend.Y не будет иметь эффекта.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Установить позицию легенды
            chart.Legend.Position = LegendPositionType.Left;

            // Сохраните книгу
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


