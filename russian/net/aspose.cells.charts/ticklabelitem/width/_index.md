---
title: "TickLabelItem.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabelItem. Ширина элемента Ticklabel как отношение к ширине диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/ticklabelitem/width/
---
## TickLabelItem.Width property

Ширина элемента Ticklabel как отношение к ширине диаграммы.

```csharp
public double Width { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyWidthDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            // Получить доступ к элементам меток делений
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Продемонстрировать свойство Width, добавляя фигуры, соответствующие размерам метки деления
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Добавить прямоугольник, соответствующий размерам подписи деления (используя свойство Width)
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Сохраните книгу
            workbook.Save("TickLabelItemWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


