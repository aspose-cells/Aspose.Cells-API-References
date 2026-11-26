---
title: "Axis.CustomDisplayUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает пользовательское значение для единицы отображения"
type: docs
url: /ru/net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Указывает пользовательское значение для единицы отображения.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCustomDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000000);
            worksheet.Cells["B3"].PutValue(20000000);
            worksheet.Cells["B4"].PutValue(30000000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить пользовательскую единицу отображения для оси значений
            chart.ValueAxis.CustomDisplayUnit = 1.0E7;
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Custom;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


