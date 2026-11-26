---
title: "Chart.WallsAndGridlines2D"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Истина, если линии сетки рисуются двумерно на 3D‑диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/wallsandgridlines2d/
---
## Chart.WallsAndGridlines2D property

Истина, если линии сетки рисуются в двумерном виде на 3‑D диаграмме.

```csharp
public bool WallsAndGridlines2D { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsAndGridlines2DDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(15);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство WallsAndGridlines2D
            chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
            Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);

            // Сохраните книгу
            workbook.Save("WallsAndGridlines2DDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


