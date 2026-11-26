---
title: "SparklineGroup.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает тип спарклайна группы спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Указывает тип спарклайна группы спарклайнов.

```csharp
public SparklineType Type { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
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

            // Создайте группу спарклайнов с типом Column
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Измените тип спарклайна на Line
            group.Type = SparklineType.Line;

            // Добавить спарклайн в группу
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Сохраните книгу
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


