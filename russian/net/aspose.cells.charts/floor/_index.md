---
title: "Класс Floor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Floor. Инкапсулирует объект, представляющий пол 3D‑диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/floor/
---
## Floor class

Инкапсулирует объект, представляющий основание 3‑D диаграммы.

```csharp
public class Floor : Area
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Получает или задает фоновый Color элемента [`Area`](../../aspose.cells.drawing/area/). (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Получает или задает границу [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Представляет объект [`FillFormat`](../../aspose.cells.drawing/area/fillformat/), содержащий свойства форматирования заливки для указанной диаграммы или формы. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Получает или задает foreground Color. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Представляет форматирование области. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Если свойство равно true и значение точки диаграммы отрицательное, foreground color и background color будут обменены. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Создайте объект рабочей книги
            Workbook workbook = new Workbook();

            // Получить коллекцию ячеек
            Cells cells = workbook.Worksheets[0].Cells;

            // Поместить значения в ячейки
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Получить коллекцию диаграмм
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Добавить новую диаграмму
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Получить только что добавленную диаграмму
            Chart chart = charts[index];

            // Установить nseries диаграммы
            chart.NSeries.Add("A1:A3", true);

            // Показать подписи данных
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Получить пол диаграммы
            Floor floor = chart.Floor;

            // Установить границу пола красным
            floor.Border.Color = Color.Red;

            // Установить формат заливки
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Установить дополнительные свойства
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Сохранить файл
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### См. также

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


