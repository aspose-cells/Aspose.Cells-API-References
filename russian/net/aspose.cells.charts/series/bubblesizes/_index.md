---
title: "Series.BubbleSizes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает или задаёт значения размеров пузырей серии диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Получает или задает значения размеров пузырей серии диаграммы.

```csharp
public string BubbleSizes { get; set; }
```

### Примечания

Только для Bubble или Bubble3D.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример данных для пузырчатой диаграммы
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Добавить пузырчатую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите данные серии, используя свойство BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Сохраните книгу
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


