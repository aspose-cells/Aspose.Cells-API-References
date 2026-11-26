---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineGroupCollection. Очищает группы sparkline, которые перекрывают область ячеек"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Очищает группы спарклайнов, которые перекрывают область ячеек.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Указывает область ячеек |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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
                // Вызовите метод ClearSparklineGroups с параметром CellArea
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Проверьте количество групп sparkline после очистки
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


