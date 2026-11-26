---
title: "ChartFrame.Y"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает координату y верхнего левого угла в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Возвращает или задает координату y верхнего левого угла в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Примечания

Как преобразовать единицы 1/4000 в пиксели? Y в пикселях = Y * Chart.ChartObject.Height / 4000d;

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.YRatioToChart. Y = YRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Получите заголовок диаграммы и задайте позицию Y
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Сохраните книгу
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


