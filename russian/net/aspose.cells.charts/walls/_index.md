---
title: "Класс Walls"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Walls. Инкапсулирует объект, представляющий стены 3D‑диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/walls/
---
## Walls class

Инкапсулирует объект, представляющий стены 3‑D диаграммы.

```csharp
public class Walls : Floor
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Получает или задает фоновый Color элемента [`Area`](../../aspose.cells.drawing/area/). (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Получает или задает границу [`Line`](../../aspose.cells.drawing/line/). (Унаследовано от [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Получает координату x левого нижнего угла центра стены в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Получает координату x нижнего левого угла центра стены в пикселях после вызова метода Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Получает координату y левого нижнего угла центра стены в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Получает координату y левого нижнего угла центра стены в пикселях после вызова метода Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Получает глубину от передней к задней в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Получает глубину спереди назад в пикселях после вызова метода Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Представляет объект [`FillFormat`](../../aspose.cells.drawing/area/fillformat/), содержащий свойства форматирования заливки для указанной диаграммы или формы. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Получает или задает foreground Color. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Представляет форматирование области. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Получает высоту сверху вниз в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Получает высоту сверху вниз в пикселях после вызова метода Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Если свойство равно true и значение точки диаграммы отрицательное, foreground color и background color будут обменены. (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). (Унаследовано от [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Получает ширину слева направо в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Получает ширину слева направо в пикселях после вызова метода Chart.Calculate(). |

## Методы

| Имя | Описание |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Получает количество точек куба после вызова метода Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Получает координату x вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми. |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Получает координату y вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
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

            // Добавьте 3D‑диаграмму в лист.
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы обновить её свойства.
            chart.Calculate();

            // Получите доступ к стенам 3D‑диаграммы.
            Walls walls = chart.Walls;

            // Установите свойства стен.
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Получите доступ к границе стен и установите её свойства.
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Выведите некоторые свойства стен.
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Сохраните книгу
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### См. также

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


