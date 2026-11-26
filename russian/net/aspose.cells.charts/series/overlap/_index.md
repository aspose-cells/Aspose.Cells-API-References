---
title: "Series.Overlap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Указывает, как расположены столбцы и колонки. Может принимать значение от 100 до 100. Применяется только к 2D столбчатым и 2D колонным диаграммам"
type: docs
url: /ru/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Указывает, как позиционируются бары и столбцы. Может принимать значение от -100 до 100. Применяется только к 2‑D барным и 2‑D столбчатым диаграммам.

```csharp
public short Overlap { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Добавьте сгруппированную колонную диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите свойство overlap для первой серии
            chart.NSeries[0].Overlap = -40;

            // Сохраните книгу
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


