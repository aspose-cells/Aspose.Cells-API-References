---
title: "ChartArea.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или задает горизонтальное смещение от столбца нижнего правого угла в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Получает или задает горизонтальное смещение от столбца нижнего правого угла в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте вместо него свойство ChartArea.WidthRatioToChart. Width = WidthRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите область диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Установить и продемонстрировать свойство Width
            Console.WriteLine("Original Width: " + chartArea.Width);
            chartArea.Width = 800; // Set new width
            Console.WriteLine("Modified Width: " + chartArea.Width);

            // Сохраните книгу
            workbook.Save("ChartAreaWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


