---
title: "ChartDataTable.HasBorderOutline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. Истина, если у таблицы данных диаграммы есть контурные границы"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/hasborderoutline/
---
## ChartDataTable.HasBorderOutline property

Истина, если у таблицы данных диаграммы есть границы контура

```csharp
[Obsolete("Use ChartDataTable.HasOutlineBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderOutline { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasOutlineBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderOutlineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Включить и настроить таблицу данных
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Продемонстрировать свойство HasBorderOutline
            chartTable.HasBorderOutline = true;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.Font.Color = Color.Blue;

            workbook.Save("ChartDataTableWithBorderOutline.xlsx");
        }
    }
}
```

### См. также

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


