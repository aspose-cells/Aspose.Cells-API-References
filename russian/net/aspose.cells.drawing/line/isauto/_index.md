---
title: "Line.IsAuto"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает, автоматически ли назначен этот стиль линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Указывает, автоматически ли назначен этот стиль линии.

```csharp
public bool IsAuto { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Добавить линейную диаграмму
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Установить диапазон данных диаграммы
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Получите доступ к свойствам линии серии
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Отобразите текущее значение IsAuto
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Установите IsAuto в true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Установите IsAuto в false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Сохраните книгу
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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


