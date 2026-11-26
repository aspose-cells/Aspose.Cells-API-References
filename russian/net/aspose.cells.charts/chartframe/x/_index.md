---
title: "ChartFrame.X"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает координату x верхнего левого угла в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Получает или задает координату x верхнего левого угла в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Примечания

Как преобразовать единицы 1/4000 в пиксели? X в пикселях = X * Chart.ChartObject.Width / 4000d;

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.XRatioToChart. X = XRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Добавить диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Добавьте серии и задайте значения X/Y
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Добавьте линию тренда
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Настройте подписи данных
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // Продемонстрируйте использование свойства X
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Сохраните книгу
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


