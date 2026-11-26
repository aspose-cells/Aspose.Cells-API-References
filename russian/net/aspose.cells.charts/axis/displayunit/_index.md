---
title: "Axis.DisplayUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет метку единицы измерения для указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Представляет метку единицы для указанной оси.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["B3"].PutValue(20000);
            worksheet.Cells["B4"].PutValue(30000);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить единицу отображения для оси значений в тысячах
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

            // Сохраните книгу
            workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


