---
title: "Line.BeginArrowLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает длину наконечника стрелки для начала линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Указывает длину наконечника стрелки для начала линии.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте простые данные для диаграммы
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

                // Установите BeginArrowLength в значение Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Прочитайте и отобразите текущее значение BeginArrowLength
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Сохраните рабочую книгу (необязательно, только для завершения демонстрации)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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


