---
title: "Line.EndArrowLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает длину наконечника стрелки для конца линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Указывает длину наконечника стрелки для конца линии.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
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
                // Добавьте диаграмму, чтобы продемонстрировать свойства линии
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Получите свойства линии из границы серии диаграммы
                Line line = chart.NSeries[0].Border;

                // Установите тип наконечника стрелки, чтобы продемонстрировать EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Отобразите текущее значение EndArrowLength
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Установите новое значение EndArrowLength
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Сохраните книгу
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


