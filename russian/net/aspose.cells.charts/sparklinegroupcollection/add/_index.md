---
title: "SparklineGroupCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineGroupCollection. Добавляет SparklineGroup со Sparkline в коллекцию"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Добавляет [`SparklineGroup`](../../sparklinegroup/) с [`Sparkline`](../../sparkline/) в коллекцию.

```csharp
public int Add(SparklineType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | SparklineType | Указывает тип группы Sparkline. |

### Возвращаемое значение

[`SparklineGroup`](../../sparklinegroup/) object index.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для спарклайнов
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Получить коллекцию групп sparkline
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Вызовите метод Add с параметром SparklineType
                int index = sparklineGroups.Add(SparklineType.Line);

                // Настроить группу sparkline
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Добавляет [`SparklineGroup`](../../sparklinegroup/) с некоторыми [`Sparkline`](../../sparkline/) в коллекцию.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | SparklineType | Указывает тип группы Sparkline. |
| dataRange | String | Указывает диапазон данных группы sparkline. |
| isVertical | Boolean | Указывает, отображать ли sparklines из диапазона данных по строкам или по столбцам. |
| locationRange | CellArea | Указывает, где размещать спарклайны. |

### Возвращаемое значение

[`SparklineGroup`](../../sparklinegroup/) object index.

### Примечания

Этот метод также создаст sparklines. Если *isVertical* истинно, количество строк в dataRange и locationRange должно совпадать. Если *isVertical* ложно, количество столбцов в dataRange и locationRange должно совпадать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для спарклайнов
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Добавить группу sparkline с указанными параметрами
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


