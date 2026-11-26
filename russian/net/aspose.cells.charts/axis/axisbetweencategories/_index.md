---
title: "Axis.AxisBetweenCategories"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет, пересекает ли ось значений ось категорий между категориями"
type: docs
url: /ru/net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

Представляет, пересекает ли ось значений ось категорий между категориями.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### Примечания

Это свойство применяется только к осям категорий и не применяется к 3‑D диаграммам.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisBetweenCategoriesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Categories");
            worksheet.Cells["B1"].PutValue("Values");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
                worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите данные диаграммы
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Настроить категориальную ось
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false; // Core property demonstration
            categoryAxis.TickLabels.RotationAngle = 45;

            // Сохраните книгу
            workbook.Save("AxisBetweenCategoriesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


