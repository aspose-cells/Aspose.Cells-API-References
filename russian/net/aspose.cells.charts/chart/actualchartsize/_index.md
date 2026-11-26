---
title: "Chart.ActualChartSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает фактический размер диаграммы в пикселях"
type: docs
url: /ru/net/aspose.cells.charts/chart/actualchartsize/
---
## Chart.ActualChartSize property

Получает фактический размер диаграммы в пикселях.

```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Chart.GetActualSize(). Это свойство будет удалено через 12 месяцев, начиная с июля 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyActualChartSizeDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Продемонстрировать использование ActualChartSize
            Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");

            // Добавьте фигуру, размер которой основан на ActualChartSize
            Shape shape = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle,
                PlacementType.Move,
                0.5,  // x position (relative)
                0.5,  // y position (relative)
                0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
                0.6   // height
            );
            shape.Fill.SolidFill.Color = Color.Blue;

            // Сохраните книгу
            workbook.Save("ChartWithActualSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


