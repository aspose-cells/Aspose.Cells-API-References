---
title: "SparklineGroup.DisplayHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает, показывать ли данные в скрытых строках и столбцах"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Указывает, следует ли показывать данные в скрытых строках и столбцах.

```csharp
public bool DisplayHidden { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyDisplayHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определить расположение спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавить группу спарклайнов
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Добавить спарклайн в группу
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Настроить внешний вид спарклайна
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // Продемонстрировать свойство DisplayHidden
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Сохраните книгу
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


