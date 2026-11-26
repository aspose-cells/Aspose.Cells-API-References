---
title: "SparklineGroupCollection.ClearSparklines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineGroupCollection. Очищает спарклайны, находящиеся в области ячеек"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Очищает спарклайны, находящиеся внутри области ячеек.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Указывает область ячеек |

### Примечания

[`SparklineGroup`](../../sparklinegroup/) will be removed too if it does not contains any [`Sparkline`](../../sparkline/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определите CellArea для спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавьте группу спарклайнов в лист
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            try
            {
                // Вызовите метод ClearSparklines с параметром CellArea
                sheet.SparklineGroups.ClearSparklines(ca);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


