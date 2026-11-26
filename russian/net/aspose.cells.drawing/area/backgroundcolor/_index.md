---
title: "Area.BackgroundColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Получает или задаёт фоновой Color области Area"
type: docs
url: /ru/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Получает или задаёт фоновой Color элемента [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Установите фоновый цвет для области оси категорий
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Отобразить фоновый цвет
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Сохраните книгу
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


