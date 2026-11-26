---
title: "Series.ShowNegativeBubbles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. True, если отрицательные пузыри отображаются для группы диаграмм. Действительно только для bubble charts"
type: docs
url: /ru/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

Истина, если для группы диаграммы отображаются отрицательные пузыри. Действительно только для пузырьковых диаграмм.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример данных для пузырчатой диаграммы
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Добавить пузырчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // Получите доступ к первой серии и задайте свойство ShowNegativeBubbles
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


