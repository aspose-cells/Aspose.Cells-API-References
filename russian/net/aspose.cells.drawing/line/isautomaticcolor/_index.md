---
title: "Line.IsAutomaticColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает, автоматически ли назначен цвет линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Указывает, автоматически ли назначен цвет линии.

```csharp
public bool IsAutomaticColor { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Добавить линейную диаграмму
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Получите доступ к линии (границе) первой серии
                Line seriesLine = chart.NSeries[0].Border;

                // Прочитайте и отобразите значение свойства IsAutomaticColor
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Сохраните книгу
                workbook.Save("IsAutomaticColorDemo.xlsx");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


