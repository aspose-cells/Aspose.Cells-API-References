---
title: "Chart.GapWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задает расстояние между группами столбцов или полос в процентах от их ширины. Значение этого свойства должно быть от 0 до 500"
type: docs
url: /ru/net/aspose.cells.charts/chart/gapwidth/
---
## Chart.GapWidth property

Возвращает или задает пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500.

```csharp
public int GapWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapWidthDemo
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

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство GapWidth
            Console.WriteLine("Original GapWidth: " + chart.GapWidth);
            chart.GapWidth = 150; // Set gap width to 150% of default
            Console.WriteLine("Modified GapWidth: " + chart.GapWidth);

            // Сохраните книгу
            workbook.Save("ChartGapWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


