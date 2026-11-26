---
title: "Chart.Perspective"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задаёт перспективу трёхмерного представления диаграммы. Должно быть в диапазоне от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes равно True"
type: docs
url: /ru/net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Возвращает или задает перспективу трехмерного просмотра диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes равно True.

```csharp
public short Perspective { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите свойства перспективы 3D‑диаграммы
            chart.Perspective = 30; // Perspective angle (0-100)
            chart.RotationAngle = 15; // Rotation angle
            chart.Elevation = 20; // Elevation angle
            chart.RightAngleAxes = false; // Enable perspective projection
            chart.AutoScaling = true; // Auto scale the chart

            // Сохраните книгу
            workbook.Save("ChartPerspectiveDemo.xlsx");

            Console.WriteLine("Chart with perspective settings created successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


