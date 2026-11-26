---
title: "Area.ForegroundColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Получает или задаёт foreground Color"
type: docs
url: /ru/net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Получает или задает цвет переднего плана.

```csharp
public Color ForegroundColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyForegroundColorDemo
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

            // Установите разные foreground цвета для каждой области серии
            chart.NSeries[0].Area.ForegroundColor = Color.FromArgb(79, 129, 189);
            chart.NSeries[1].Area.ForegroundColor = Color.FromArgb(192, 80, 77);

            // Сохраните книгу
            workbook.Save("AreaForegroundColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


