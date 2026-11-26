---
title: "Series.SizeRepresents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает или задает, что представляет размер пузыря на пузырчатой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Получает или задает, что представляет размер пузыря на пузырьковой диаграмме.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Примечания

BubbleSizeRepresents.SizeIsArea означает, что значение [`BubbleSizes`](../bubblesizes/) является площадью пузыря. BubbleSizeRepresents.SizeIsWidth означает, что значение [`BubbleSizes`](../bubblesizes/) является шириной пузыря.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить пример данных для пузырчатой диаграммы
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Добавить пузырчатую диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Установить данные серии
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // Установить свойство SizeRepresents
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Сохраните книгу
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


