---
title: "ChartPoint.ShapeHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает высоту в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Получает высоту в единицах 1/4000 от высоты диаграммы после вызова метода Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы обеспечить доступность свойств фигур.
            chart.Calculate();

            // Получите первую точку в первой серии.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение ShapeHeight (в 1/4000 высоты диаграммы).
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Примечание: ShapeHeight только для чтения, поэтому установить его напрямую нельзя.
            // Чтобы изменить высоту, необходимо изменить размер диаграммы или другие свойства.

            // Продемонстрируйте эффект, изменив высоту диаграммы.
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Отобразите новое значение ShapeHeight после изменения высоты диаграммы.
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Сохранить результат
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


