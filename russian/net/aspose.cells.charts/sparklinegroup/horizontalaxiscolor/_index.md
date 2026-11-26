---
title: "SparklineGroup.HorizontalAxisColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает цвет горизонтальной оси в группе спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/horizontalaxiscolor/
---
## SparklineGroup.HorizontalAxisColor property

Получает и задает цвет горизонтальной оси в группе спарклайнов.

```csharp
public CellsColor HorizontalAxisColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Создать группу спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Установить цвет горизонтальной оси
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Blue;
            group.HorizontalAxisColor = axisColor;
            group.ShowHorizontalAxis = true;

            // Сохраните книгу
            workbook.Save("SparklineHorizontalAxisColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


