---
title: "SparklineGroup.ShowHighPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает, следует ли выделять наивысшие точки данных в группе спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Указывает, следует ли выделять самые высокие точки данных в группе спарклайнов.

```csharp
public bool ShowHighPoint { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHighPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Создать группу спарклайнов
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Добавить спарклайн
            group.Sparklines.Add("A1:D1", 0, 4);

            // Настроить отображение высшей точки
            group.ShowHighPoint = true;
            CellsColor highColor = workbook.CreateCellsColor();
            highColor.Color = System.Drawing.Color.Green;
            group.HighPointColor = highColor;

            // Сохранить книгу
            workbook.Save("SparklineHighPointDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


