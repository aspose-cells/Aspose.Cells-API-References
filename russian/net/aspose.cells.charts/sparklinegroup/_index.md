---
title: "Класс SparklineGroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.SparklineGroup class. Спарклайн организован в группу спарклайнов. SparklineGroup содержит переменное количество элементов спарклайна. Группа спарклайнов задает настройки отображения типа и настройки осей для спарклайнов."
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline/) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```csharp
public class SparklineGroup
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden/) { get; set; } | Указывает, следует ли показывать данные в скрытых строках и столбцах. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor/) { get; set; } | Получает и задает цвет первой точки данных в группе спарклайнов. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor/) { get; set; } | Получает и задает цвет самых высоких точек данных в группе спарклайнов. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor/) { get; set; } | Получает и задает цвет горизонтальной оси в группе спарклайнов. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/) { get; set; } | Представляет диапазон, содержащий значения дат для данных спарклайна. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor/) { get; set; } | Получает и задает цвет последней точки данных в группе спарклайнов. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight/) { get; set; } | Получает и задает толщину линии в каждом линейном спарклайне группы спарклайнов, в единицах пунктов. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor/) { get; set; } | Получает и задает цвет самых низких точек данных в группе спарклайнов. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor/) { get; set; } | Получает и задает цвет точек в каждом линейном спарклайне группы спарклайнов. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor/) { get; set; } | Получает и задает цвет отрицательных значений в группе спарклайнов. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype/) { get; set; } | Указывает, как отображать пустые ячейки. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft/) { get; set; } | Указывает, отображаются ли данные графика справа налево. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle/) { get; set; } | Получает и задает тип предустановленного стиля группы спарклайнов. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor/) { get; set; } | Получает и задает цвет спарклайнов в группе спарклайнов. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint/) { get; set; } | Указывает, следует ли выделять первую точку данных в группе спарклайнов. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint/) { get; set; } | Указывает, следует ли выделять самые высокие точки данных в группе спарклайнов. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis/) { get; set; } | Указывает, следует ли отображать горизонтальную ось спарклайна. Горизонтальная ось появляется, если у спарклайна есть данные, пересекающие нулевую ось. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint/) { get; set; } | Указывает, следует ли выделять последнюю точку данных в группе спарклайнов. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint/) { get; set; } | Указывает, следует ли выделять самые низкие точки данных в группе спарклайнов. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers/) { get; set; } | Указывает, следует ли выделять каждую точку в каждой линейной спарклайне в группе спарклайнов. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints/) { get; set; } | Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection/) { get; } | (**Obsolete.**) Получает коллекцию объектов [`Sparkline`](../sparkline/). |
| [Sparklines](../../aspose.cells.charts/sparklinegroup/sparklines/) { get; } | Получает коллекцию объектов [`Sparkline`](../sparkline/). |
| [Type](../../aspose.cells.charts/sparklinegroup/type/) { get; set; } | Указывает тип спарклайна группы спарклайнов. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/) { get; set; } | Получает и задает пользовательское максимальное значение вертикальной оси. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/) { get; set; } | Представляет тип максимального значения вертикальной оси. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue/) { get; set; } | Получает и задает пользовательское минимальное значение вертикальной оси. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/) { get; set; } | Представляет тип минимального значения вертикальной оси. |

## Методы

| Имя | Описание |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges/)(string, bool, CellArea) | Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. Этот метод очистит исходные элементы спарклайнов в группе и создаст новые элементы спарклайнов для новых диапазонов. |
| [SetVerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/setverticalaxismaxvalue/)(SparklineAxisMinMaxType, double) | Устанавливает пользовательское максимальное значение вертикальной оси спарклайна с указанным типом значения оси. |
| [SetVerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/setverticalaxisminvalue/)(SparklineAxisMinMaxType, double) | Устанавливает пользовательское минимальное значение вертикальной оси спарклайна с указанным типом значения оси. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupDemo
    {
        public static void SparklineGroupExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определите CellArea для спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавьте группу спарклайнов в лист
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Добавьте спарклайны в группу
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Создайте CellsColor для цвета серии
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Установите, чтобы высокие точки были окрашены в зеленый, а низкие — в красный
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            group.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            group.LowPointColor = lowPointColor;

            // Установите толщину линии
            group.LineWeight = 1.0;

            // Установить дополнительные свойства
            group.PresetStyle = SparklinePresetStyleType.Style1;
            group.Type = SparklineType.Line;
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
            group.DisplayHidden = true;
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            group.PlotRightToLeft = false;
            CellsColor horizontalAxisColor = workbook.CreateCellsColor();
            horizontalAxisColor.Color = Color.Gray;
            group.HorizontalAxisColor = horizontalAxisColor;

            group.ShowHorizontalAxis = true;
            group.HorizontalAxisDateRange = "A1:D1";
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMinValue = 0.0;

            // Сохраните книгу
            workbook.Save("SparklineGroupExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


