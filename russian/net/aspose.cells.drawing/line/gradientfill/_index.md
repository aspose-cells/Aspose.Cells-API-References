---
title: "Line.GradientFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Представляет градиентную заливку"
type: docs
url: /ru/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Представляет градиентную заливку.

```csharp
public GradientFill GradientFill { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Получите первую точку первой серии
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Получите доступ к объекту Line (граница) точки
                Line line = point.Border;

                // Прочитайте свойство GradientFill (только для чтения)
                GradientFill gradient = line.GradientFill;

                // Отобразите детали текущей градиентной заливки
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Измените градиент, используя предоставленные методы
                // Используйте приведение к значению перечисления по умолчанию, чтобы избежать ссылки на несуществующий элемент
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Сохраните книгу
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


