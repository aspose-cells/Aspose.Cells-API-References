---
title: "ChartFrame.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает ширину рамки в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Получает или задает ширину рамки в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Примечания

Как преобразовать единицы 1/4000 в пиксели? Ширина в пикселях = Ширина * Chart.ChartObject.Height / 4000d;

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.WidthRatioToChart вместо него. Ширина = WidthRatioToChart * 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
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

            // Добавьте диаграмму и получите её кадр
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Установить и отобразить исходную ширину
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Изменить ширину
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Сохраните книгу
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


