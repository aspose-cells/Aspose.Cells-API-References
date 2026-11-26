---
title: "ChartDataTable.HasBorderVertical"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. True, если у таблицы данных диаграммы есть вертикальные границы ячеек"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/hasbordervertical/
---
## ChartDataTable.HasBorderVertical property

Истина, если у таблицы данных диаграммы есть вертикальные границы ячеек

```csharp
[Obsolete("Use ChartDataTable.HasVerticalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderVertical { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ChartDataTable.HasVerticalBorder. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderVerticalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderHorizontal = true;

            workbook.Save("ChartDataTable_HasBorderVertical.xlsx");
        }
    }
}
```

### См. также

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


