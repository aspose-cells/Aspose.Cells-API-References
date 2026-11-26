---
title: "Series.Area"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Представляет фоновую область объекта Series"
type: docs
url: /ru/net/aspose.cells.charts/series/area/
---
## Series.Area property

Представляет область фона объекта Series.

```csharp
public Area Area { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyAreaDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к первой серии и задайте текстуру области
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Texture = TextureType.Stationery;

            // Сохраните книгу
            workbook.Save("SeriesPropertyAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


