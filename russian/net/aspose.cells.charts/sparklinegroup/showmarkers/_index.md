---
title: "SparklineGroup.ShowMarkers"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает, следует ли выделять каждую точку в каждой линейной спарклайне группы спарклайнов."
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/showmarkers/
---
## SparklineGroup.ShowMarkers property

Указывает, следует ли выделять каждую точку в каждой линейной спарклайне в группе спарклайнов.

```csharp
public bool ShowMarkers { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowMarkersDemo
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

            // Добавить спарклайн
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Настроить внешний вид спарклайна
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            group.ShowMarkers = true;
            
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // Сохраните книгу
            workbook.Save("SparklineWithMarkers.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


