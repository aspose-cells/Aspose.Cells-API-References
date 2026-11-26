---
title: "Area.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Возвращает или задаёт степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AreaPropertyTransparencyDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к первой серии
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Продемонстрировать свойство Transparency
            Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
            Console.WriteLine("Initial border transparency: " + series.Border.Transparency);

            // Изменить значения прозрачности
            series.Area.Transparency = 0.5; // 50% transparent
            series.Border.Transparency = 0.2; // 20% transparent

            Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
            Console.WriteLine("Modified border transparency: " + series.Border.Transparency);

            // Сохраните книгу
            workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


