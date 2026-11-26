---
title: "TickLabels.TickLabelItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Возвращает отображаемые метки делений оси"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/ticklabelitems/
---
## TickLabels.TickLabelItems property

Получает отображаемые подписи делений оси.

```csharp
public TickLabelItem[] TickLabelItems { get; }
```

### Примечания

Доступно только после вызова метода [`Calculate`](../../chart/calculate/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTickLabelItemsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Вычислить диаграмму
            chart.Calculate();

            // Получить категориальную ось и её метки делений
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Добавить фигуры для обозначения позиции каждой метки деления
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Добавить прямоугольник вокруг каждой метки деления
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;
            }

            // Сохраните книгу
            workbook.Save("TickLabelItemsDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


