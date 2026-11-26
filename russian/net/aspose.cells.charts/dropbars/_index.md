---
title: "Класс DropBars"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.DropBars. Представляет восходящие и нисходящие столбцы в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/dropbars/
---
## DropBars class

Представляет верхние и нижние столбцы в диаграмме.

```csharp
public class DropBars
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Получает [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Получает границу [`Line`](../../aspose.cells.drawing/line/). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте NSeries (источник данных диаграммы) к диаграмме, охватывающий ячейки от "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Включить восходящие и нисходящие столбцы
            chart.NSeries[0].HasUpDownBars = true;

            // Получите доступ к объекту DropBars
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Настройте внешний вид восходящих столбцов
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Настройте внешний вид нисходящих столбцов
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Сохраните книгу
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


