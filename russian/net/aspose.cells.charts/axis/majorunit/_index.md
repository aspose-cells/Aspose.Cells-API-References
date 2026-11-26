---
title: "Axis.MajorUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет основные единицы измерения для оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Представляет основные единицы для оси.

```csharp
public double MajorUnit { get; set; }
```

### Примечания

Основные единицы должны быть больше нуля.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Получить категориальную ось
            Axis axis = chart.CategoryAxis;

            // Отобразить начальную основную единицу
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Установить новую основную единицу
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Сохраните книгу
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


