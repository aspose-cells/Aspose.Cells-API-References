---
title: "ChartPoint.ShapeX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату x верхнего левого угла в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Получает координату x верхнего левого угла в единицах 1/4000 от ширины диаграммы после вызова метода Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Выполните расчёт диаграммы, чтобы убедиться, что ShapeX заполнен.
            chart.Calculate();

            // Получите первую точку в первой серии.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите значение ShapeX (1/4000 ширины диаграммы).
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Продемонстрируйте использование ShapeX для позиционирования элементов относительно точки диаграммы.
            // Примечание: Поскольку ShapeX доступен только для чтения, мы не можем изменить его напрямую,
            // но мы можем использовать его для позиционирования других элементов.
            if (point.ShapeX > 0)
            {
                // Добавьте текстовое поле, выровненное по позиции X точки диаграммы.
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Сохранить результат
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


