---
title: "Worksheet.SparklineGroups"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает группы спарклайнов на листе"
type: docs
url: /ru/net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Получает группы спарклайнов в листе.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Примеры

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySparklineGroupsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполнить тестовыми данными
            Cells cells = sheet.Cells;
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    cells[i, j].Value = (i + 1) * (j + 1);
                }
            }

            // Добавить группу спарклайнов
            int groupIndex = sheet.SparklineGroups.Add(
                0, // Line sparkline type code
                "A1:D4", 
                false, 
                CellArea.CreateCellArea("F1", "F4")
            );

            workbook.Save("output_sparklines.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


