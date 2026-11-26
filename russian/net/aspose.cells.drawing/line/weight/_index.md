---
title: "Line.Weight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Получает или задает WeightType линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Получает или задает [`WeightType`](../../weighttype/) линии.

```csharp
public WeightType Weight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightDemo
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

            // Получите доступ к области диаграммы и задайте толщину границы
            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.MediumLine;

            // Сохраните книгу
            workbook.Save("LinePropertyWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


