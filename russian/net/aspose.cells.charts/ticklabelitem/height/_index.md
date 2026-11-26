---
title: "TickLabelItem.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabelItem. Высота элемента подписи деления как отношение к высоте диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/ticklabelitem/height/
---
## TickLabelItem.Height property

Высота элемента Ticklabel как отношение к высоте диаграммы.

```csharp
public double Height { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyHeightDemo
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

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            // Доступ к меткам делений оси категорий
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Добавить фигуры для визуализации высот элементов подписи деления
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Добавить прямоугольник, показывающий границы элемента подписи деления
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;

                // Добавить текст, показывающий значение высоты
                Shape textShape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.TextBox,
                    PlacementType.Move,
                    item.X,
                    item.Y - 0.05, // Position above the tick label
                    0.1,
                    0.05);
                
                textShape.Text = $"H: {item.Height:F4}";
                textShape.Fill.SolidFill.Transparency = 1;
            }

            // Сохраните книгу
            workbook.Save("TickLabelItemHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


