---
title: "Line.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Возвращает или задает степень прозрачности линии в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Возвращает или задает степень прозрачности линии значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Добавьте линейную диаграмму, чтобы продемонстрировать свойства линии
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Получите свойства линии из границы серии диаграммы
                Line line = chart.NSeries[0].Border;

                // Отобразить текущее значение Transparency
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Установите новое значение Transparency (0.0 = непрозрачный, 1.0 = прозрачный)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Сохраните книгу
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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


