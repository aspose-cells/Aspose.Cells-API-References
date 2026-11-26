---
title: "Класс TickLabelItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.TickLabelItem. Представляет метку деления на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Представляет метку деления на диаграмме.

```csharp
public class TickLabelItem
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Высота элемента Ticklabel как отношение к высоте диаграммы. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Ширина элемента Ticklabel как отношение к ширине диаграммы. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | Координаты X элемента Ticklabel как отношение к ширине диаграммы. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Координаты Y элемента Ticklabel как отношение к высоте диаграммы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
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

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            // Доступ к меткам делений оси категорий
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Добавить фигуры для обозначения позиции каждой метки деления
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Добавить прямоугольник вокруг метки деления
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Добавить круг рядом с меткой деления
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Сохраните книгу
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


