---
title: "Sparkline.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Sparkline. Возвращает индекс строки спарклайна"
type: docs
url: /ru/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Получает индекс строки спарклайна.

```csharp
public int Row { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Добавить спарклайн в строке 0, столбце 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Отображать позицию строки (только для чтения)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Чтобы изменить позицию, необходимо удалить и заново создать спарклайн
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Сохранить книгу
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


