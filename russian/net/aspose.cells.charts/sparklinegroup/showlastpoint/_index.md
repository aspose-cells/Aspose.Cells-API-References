---
title: "SparklineGroup.ShowLastPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает, следует ли выделять последнюю точку данных в группе спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/showlastpoint/
---
## SparklineGroup.ShowLastPoint property

Указывает, следует ли выделять последнюю точку данных в группе спарклайнов.

```csharp
public bool ShowLastPoint { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowLastPointDemo
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

            // Создать группу спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Добавить спарклайн
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Настроить внешний вид спарклайна
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;
            group.LineWeight = 1.0;

            // Включить и раскрасить последнюю точку
            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            // Сохраните книгу
            workbook.Save("SparklineShowLastPointDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


