---
title: "Axis.MaxValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет максимальное значение на оси значений"
type: docs
url: /ru/net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Представляет максимальное значение на оси значений.

```csharp
public object MaxValue { get; set; }
```

### Примечания

Тип maxValue может быть только double или DateTime

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(50);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить максимальное значение оси значений
            chart.ValueAxis.MaxValue = 60;

            // Сохраните книгу
            workbook.Save("AxisPropertyMaxValueDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


