---
title: "TickLabelItem.Y"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabelItem. Координата Y элемента Ticklabel как отношение к высоте диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Координаты Y элемента Ticklabel как отношение к высоте диаграммы.

```csharp
public double Y { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // Установить данные оси категорий, используя NSERIES вместо CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Вычислить диаграмму, чтобы гарантировать генерацию меток делений
            chart.Calculate();

            // Получить элементы меток делений с оси категорий
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Продемонстрировать использование свойства Y, добавляя фигуры, выровненные с метками делений
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Добавить прямоугольник в каждой позиции Y метки деления
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Сохраните книгу
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


