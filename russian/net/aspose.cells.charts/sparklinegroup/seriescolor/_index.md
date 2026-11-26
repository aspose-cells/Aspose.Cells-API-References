---
title: "SparklineGroup.SeriesColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает цвет спарклайнов в группе спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

Получает и задает цвет спарклайнов в группе спарклайнов.

```csharp
public CellsColor SeriesColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySeriesColorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Пример данных
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(8);
            ws.Cells["A3"].PutValue(3);
            
            // Создать группу спарклайнов
            CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
            int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
            
            // Установить цвет серии
            SparklineGroup group = ws.SparklineGroups[index];
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;
            
            wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


