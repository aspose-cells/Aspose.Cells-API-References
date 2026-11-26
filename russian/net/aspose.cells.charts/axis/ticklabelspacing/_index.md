---
title: "Axis.TickLabelSpacing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет количество категорий или рядов между метками делений. Применяется только к категориальным и рядовым осям"
type: docs
url: /ru/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Представляет количество категорий или рядов между метками делений. Применяется только к осям категорий и рядов.

```csharp
public int TickLabelSpacing { get; set; }
```

### Примечания

Число должно быть в диапазоне от 1 до 31999.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите данные диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Настроить интервал меток делений оси
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


