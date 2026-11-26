---
title: "Chart.Walls"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает объект Walls, представляющий стены 3D‑диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Возвращает объект `Walls`, представляющий стены 3‑D диаграммы.

```csharp
public Walls Walls { get; }
```

### Примечания

Это свойство не применяется к 3-D круговым диаграммам.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Создайте цилиндрическую столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Настройте базовые параметры диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Настройте свойства стен
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Сохранить результат
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


