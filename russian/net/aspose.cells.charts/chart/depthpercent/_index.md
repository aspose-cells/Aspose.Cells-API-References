---
title: "Chart.DepthPercent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Представляет глубину 3D‑диаграммы в процентах от ширины диаграммы в диапазоне от 20 до 2000 процентов"
type: docs
url: /ru/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов).

```csharp
public int DepthPercent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить свойство DepthPercent (управляет глубиной 3D‑диаграммы в процентах от ширины диаграммы)
            chart.DepthPercent = 150; // 150% depth

            // Сохраните книгу
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


