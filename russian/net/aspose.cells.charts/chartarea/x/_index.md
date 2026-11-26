---
title: "ChartArea.X"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или задает горизонтальное смещение от столбца верхнего левого угла в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Получает или задает горизонтальное смещение от столбца верхнего левого угла в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartArea.XRatioToChart вместо него. X = XRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Настройте область диаграммы
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Сохранить результат
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


