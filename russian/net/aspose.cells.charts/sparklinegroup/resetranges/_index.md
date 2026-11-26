---
title: "SparklineGroup.ResetRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineGroup. Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. Этот метод очистит оригинальные элементы спарклайнов в группе и создаст новые элементы спарклайнов для новых диапазонов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. Этот метод очистит исходные элементы спарклайнов в группе и создаст новые элементы спарклайнов для новых диапазонов.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataRange | String | Указывает новый диапазон данных группы спарклайнов. |
| isVertical | Boolean | Указывает, следует ли строить спарклайны из нового диапазона данных по строкам или по столбцам. |
| locationRange | CellArea | Указывает, где размещать спарклайны. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
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

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Подготовьте параметры для ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Вызовите ResetRanges с параметрами (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


