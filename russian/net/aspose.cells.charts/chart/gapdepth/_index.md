---
title: "Chart.GapDepth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает или задает расстояние между сериями данных в 3D‑диаграмме в процентах от ширины маркера. Значение этого свойства должно быть от 0 до 500"
type: docs
url: /ru/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Получает или задает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. Значение этого свойства должно быть от 0 до 500.

```csharp
public int GapDepth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить свойство GapDepth (управляет расстоянием между сериями данных в 3D‑диаграммах)
            chart.GapDepth = 150; // Value between 0-500

            // Сохраните книгу
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


