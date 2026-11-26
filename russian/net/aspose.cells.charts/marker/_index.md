---
title: "Класс Marker"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Marker. Представляет маркер в линейной, точечной или радиальной диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/marker/
---
## Marker class

Представляет маркер в линейной, точечной или радиальной диаграмме.

```csharp
public class Marker
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Получает [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Представляет цвет фона маркера в линейной, точечной или радиальной диаграмме. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Получает или задает тип набора фонового цвета маркера. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Получает [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Представляет цвет переднего плана маркера в линейной, точечной или радиальной диаграмме. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Получает или задает тип набора цвета переднего плана маркера. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Представляет размер маркера в единицах пунктов. Применяется к линейной диаграмме, точечной диаграмме или радиальной диаграмме. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Представляет размер маркера в пикселях. Применяется к линейным диаграммам, точечным диаграммам или радиальным диаграммам. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Представляет стиль маркера. Применяется к линейной диаграмме, точечной диаграмме или радиальной диаграмме. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить ссылку на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
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

            // Получить доступ к первой серии
            Series series = chart.NSeries[0];

            // Установить свойства маркера
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Сохраните книгу
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


