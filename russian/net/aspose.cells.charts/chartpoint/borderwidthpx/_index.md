---
title: "ChartPoint.BorderWidthPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPoint property. Получает ширину границы в пикселях после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Получает ширину границы в пикселях после вызова метода Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Добавьте диаграмму и задайте её диапазон данных
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получить первую точку диаграммы в первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить текущую ширину границы
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Примечание: BorderWidthPx только для чтения, поэтому мы не можем установить его напрямую
            // Вместо этого мы можем изменить границу через свойство Border
            if (point.Border != null)
            {
                // Измените ширину границы, установив вес с помощью перечисления WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Пересчитайте, чтобы обновить значение BorderWidthPx
            chart.Calculate();

            // Отобразить новую ширину границы в пикселях
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


