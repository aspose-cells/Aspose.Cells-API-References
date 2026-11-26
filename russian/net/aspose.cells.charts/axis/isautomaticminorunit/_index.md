---
title: "Axis.IsAutomaticMinorUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает, назначается ли мелкая единица оси автоматически"
type: docs
url: /ru/net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Указывает, назначается ли вспомогательный делитель оси автоматически.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinorUnitDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
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
            chart.SetChartDataRange("A1:B4", true);

            // Получить ось значений
            Axis valueAxis = chart.ValueAxis;

            // Продемонстрируйте свойство IsAutomaticMinorUnit
            Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            
            // Установите мелкую единицу вручную
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 2;
            Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);

            // Верните автоматический режим
            valueAxis.IsAutomaticMinorUnit = true;
            Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);

            // Сохраните книгу
            workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


